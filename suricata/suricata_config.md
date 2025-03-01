## Installation
sudo apt update && sudo apt upgrade -y \
sudo apt install -y software-properties-common \
sudo add-apt-repository -y ppa:oisf/suricata-stable \
sudo apt update \
sudo apt install -y suricata \
suricata --build-info \
sudo suricata-update \
suricata-update update-sources \
sudo ln -s /var/lib/suricata/rules /etc/suricata/rules

Suricate rules can be found under /usr/share/suricata/rules. You can copy them to /etc/suricata.

Configure the interface under af-packet and pcap. \
Set community-id to true. \
By default, rules for Modbus come with disabled. You need to activate them. \
The rules file in under /var/lib/suricata/rules.
