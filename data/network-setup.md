Display name: Router0
Model:1941
Hostname: Router


Display name: Switch0
Model: 2960-24TT
Hostname: Switch

Display name: Switch1
Model: 2960-24TT
Hostname: Switch


Display name: Server0
Model: Server-PT
IP address: 210.3.14.2

Display name: Server1
Model: Server-PT
IP address: 168.90.0.2

Display name: Server2
Model: Server-PT
IP address: 168.90.0.4


Display name: PC0
Model: PC-PT
IP address: 210.3.14.4

Display name: PC1
Model: PC-PT
IP address: 210.3.14.5

Display name: PC4
Model: PC-PT
IP address: 210.3.14.6

Display name: PC2
Model: PC-PT
IP address: 168.90.0.3

Display name: PC3
Model: PC-PT
IP address: 168.90.0.5


Display name: Laptop0
Model: Laptop-PT
IP address: 210.3.14.3


DHCP:

Switch0:

enable
cofigure terminal
ip dhcp pool Switch0
network 168.90.0.0 255.255.0.0
default-router 168.90.0.1

IP for router:
ip dhcp excluded-address 168.90.0.1

Configuring router:
interface GigabitEtherenet0/0
ip address 168.90.0.1 255.255.0.0


Switch1:

enable
cofigure terminal
ip dhcp pool Switch1
network 210.3.14.0 255.255.255.0
default-router 210.3.14.1

IP for router:
ip dhcp excluded-address 210.3.14.1

Configuring router:
interface GigabitEtherenet0/0
ip address 210.3.14.1 255.255.255.0







