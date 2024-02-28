# Server IP Address

ZABBIX_SERVER_IP="119.159.226.111"

# Install Zabbix Agent
sudo wget https://repo.zabbix.com/zabbix/6.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_6.0-4+ubuntu22.04_all.deb
sudo dpkg -i zabbix-release_6.0-4+ubuntu22.04_all.deb
sudo apt update
apt install zabbix-agent -y
# Configure Zabbix Agent
sudo sed -i "s/Server=127.0.0.1/Server=$ZABBIX_SERVER_IP/" /etc/zabbix/zabbix_agentd.conf
sudo sed -i "s/ServerActive=127.0.0.1/ServerActive=$ZABBIX_SERVER_IP/" /etc/zabbix/zabbix_agentd.conf
# Start Zabbix Agent
sudo systemctl start zabbix-agent
sudo systemctl enable zabbix-agent
sudo systemctl status zabbix-agent

echo "you have successfully insttalled zabbix agent cheers"
echo "you have successfully insttalled zabbix agent cheers"
echo "Zabbix Agent installed and configured. It is now communicating with the Zabbix Server at $ZABBIX_SERVER_IP."
sudo systemctl status zabbix-agent
