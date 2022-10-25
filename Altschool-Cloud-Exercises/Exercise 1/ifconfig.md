### VagrantFile to set DHCP

Using [this article](https://www.vagrantup.com/docs/networking/private_network) I was able to solve the section of setting private network to **DHCP**

```
 -*- mode: ruby -*-
Vagrant.configure("2") do |config|
    config.vm.network "private_network", type: "dhcp"
end
```

### Output of ifconfig

Step 1: `vagrant ssh`
Step 2: `sudo apt install net-tools`
Step 3: `ifconfig`

#### Result
```
enp0s3: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.0.2.15  netmask 255.255.255.0  broadcast 10.0.2.255
        inet6 fe80::74:c4ff:fe03:bf7e  prefixlen 64  scopeid 0x20<link>
        ether 02:74:c4:03:bf:7e  txqueuelen 1000  (Ethernet)
        RX packets 1102  bytes 340326 (340.3 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 862  bytes 120048 (120.0 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 37  bytes 3690 (3.6 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 37  bytes 3690 (3.6 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
```