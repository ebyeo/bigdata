# Configure Virtual Machine
The following instruction is based on these links https://www.tecmint.com/network-between-guest-vm-and-host-virtualbox/ and https://unix.stackexchange.com/questions/145997/trying-to-ssh-to-local-vm-ubuntu-with-putty to enable communication between the host and the virtual machines. This is required to be able to launch Zeppelin from the host machine. No static IP is configured as we are not certain if it will work between home and ISS network.
1. Install [Putty](https://www.putty.org/) on the host PC so that you can have multiple SSH sessions into the guest VM. 
2. Configure the network interface in the guest VM
3. Edit /etc/network/interfaces
```
sudo vi /etc/network/interfaces
```
4. Append the following entries:
```
auto enp0s3
iface enp0s3 inet dhcp
```
5. Restart the network interfaces 
```
sudo systemctl restart networking
```
6. Install the ssh server in the guest VM
```
sudo apt-get install openssh-server
```