## Installation
sudo apt update && sudo apt upgrade -y \
sudo apt install -y software-properties-common \
sudo add-apt-repository -y ppa:oisf/suricata-stable \
sudo apt update \
sudo apt install -y suricata \
suricata --build-info \
sudo suricata-update

Suricate rules can be found under /usr/share/suricata/rules. You can copy them to /etc/suricata.
