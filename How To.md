# What is 'How To' ?
In my journey to learn Linux, I often encountered problems that I had to fix. Here, I’m going to share their solutions; Hope this helps you!

---
# Install VMware tools
**note that "-y" means automatic yes**

    sudo apt update
    sudo apt install open-vm-tools-desktop -y

# Update/Change your repository
    sudo nano /etc/apt/sources.list

# "user is not in the sudoeris file" Error
    su -
    usermode -aG sudo [username]
    logout

# if your network sudenlly brock in your VMware machine
- Check Network Interface Status

      ip a
  Look for an interface like `eth0` or `ens33` and ensure it has an IP;  
  If you see `NO-CARRIER` or `DOWN`, restart the interface:
  
      sudo ip link set [interface name] up

- Check Default Gateway

      ip route show

  You should see a line like:  
  **default via [default gateway ip] dev [interface name]**

  If there's no default route, add it manually:
  
      sudo ip route add default via [default gateway ip] dev [interface name]

The problem I faced was that I checked this and many other things, and all of them were okay.
At this stage, If you're using VMware and your host is Windows, I suggest you check the solution below:

- vm NAT
  
  Run --> services.msc --> Vm NAT --> Start
