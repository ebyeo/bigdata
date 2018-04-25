# Install VirtualBox
1. Download and install the latest VirtualBox binaries from https://www.virtualbox.org/wiki/Downloads. After installing. launch VirtualBox to start creating an Ubuntu virtual machine.
1. Click _New_ to create a virtual machine
1. In the dialog box, enter as follow and click _Next_\
![vb-01](./docs/assets/virtualbox/vb-01.png)
1. Set the memory size to 4096 MB and click _Next_
1. Select _Create a virtual hard disk now_ and click _Create_\
![vb-02](./docs/assets/virtualbox/vb-02.png)
1. Select _VDI (VirtualBox Disk Image)_ and click _Next_
1. Select _dynamically allocated_ and click _Next_
1. Take the default name of the virtual hard disk and increase the size to 20 GB, click on the icon next to the name and select the directory to store the file, preferably in a large enough hard disk. Finally, click _Create_.\
![vb-03](./docs/assets/virtualbox/vb-03.png)
1. Click _Settings_ -> _Network_. Enable _Adapter 1_, select _Host-only Adapter_ and enable _Adapter 2_ and select _Nat Network_. Click _OK_ to complete the network setup.
