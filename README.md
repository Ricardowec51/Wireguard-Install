# Wireguard-Install

I've had so many headaches when trying to install Wireguard Server and clients, so I decided to make it myself by using the stock Wireguard app starting from Ubuntu 22.04 and a couple of scripts to download.

## SERVER INSTALL

Run this script on your Ubuntu (22.04 and up) that is to be your server:

```bash
curl -o install_wireguard.sh "https://raw.githubusercontent.com/Ricardowec51/Wireguard-Install/refs/heads/main/Wireguard%20Install/Script%20para%20Instalacion%20de%20Servidor%20WIREGUARD" && chmod +x install_wireguard.shCLIENTS CONFIGURATION

Runt this script every time you need to add a client. It will generate de conf file that you shouldt install in your client machine. It has to be run in the same machine as de one used to generate the server 

curl -o add_client.sh "https://raw.githubusercontent.com/Ricardowec51/Wireguard-Install/refs/heads/main/Wireguard%20Install/Script%20para%20instalacion%20de%20Clientes%20de%20Wireguards" && chmod +x add_client.sh && sudo ./add_client.sh
