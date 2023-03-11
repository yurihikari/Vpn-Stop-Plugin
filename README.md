# VPNStopPlugin
## Author
https://github.com/yurihikari
## Description
VPNStop is a plugin that will block VPN, OpenVPN, Proxy, Tor, Mobile, Business and Hosting connections from joining your server. It will also block any IP that is not in the whitelist.
## Commands

### Default command. Will list the available commands
```
/vpnstop
```
### Add an IP. connected player to the whitelist
```
/vpnstop add <ip|name> 
```
### Remove an IP. connected player to the whitelist
```
/vpnstop remove <ip|name>
```
### Show the help menu
```
/vpnstop help
```
### Show the plugin info
```
/vpnstop info
```

## Permissions
```yml
 # Bypass for players. Only 
  vpnstop.bypass:
    description: Allows bypassing the VPNStop plugin IP checking. OP only by default.
    default: op
  vpnstop.command.add:
    description: Allows players to add IPs to the whitelist. OP only by default.
    default: op
  vpnstop.command.remove:
    description: Allows players to remove IPs from the whitelist. OP only by default.
    default: op
  vpnstop.command.help:
    description: Allows players to see the help menu. OP only by default.
    default: op
  vpnstop.command.info:
   description: Allows players to get info about the plugin
   default: op
  vpnstop.commands:
   description: Allows players to use VPNStop commands
   default: op
 ```
 
 ## Default Config file
 ```yml
 # EDIT THOSE LINES WITH YOUR OWN API KEY AND API URL FROM PROXYCHECK.IO
api_url: "https://proxycheck.io/v2/" # API URL
api_key: "Use your own api key" # API KEY
# EDIT THOSE LINES TO CUSTOMIZE THE PLUGIN
kick_message: "Your IP is not allowed to join this server." # The message that will be sent to an unknown IP
vpn_kick_message: "You are using a VPN connection. Please disable it and try again." # The message that will be sent to a VPN IP
openvpn_kick_message: "You are using a OpenVPN connection. Please disable it and try again." # The message that will be sent to a OpenVPN IP
proxy_kick_message: "You are using a Proxy connection. Please disable it and try again." # The message that will be sent to a Proxy IP
tor_kick_message: "You are using a Tor connection. Please disable it and try again." # The message that will be sent to a Tor IP
mobile_kick_message: "You are using a Mobile (H+/4G/5G) connection. Please log using a Wi-Fi connection and try again." # The message that will be sent to a Mobile IP
business_kick_message: "You are using a Business connection. Please log using your own Wi-Fi connection and try again." # The message that will be sent to a Business IP
hosting_kick_message: "You are using a Hosting connection. Please log using your own Wi-Fi connection and try again." # The message that will be sent to a Hosting IP
# EDIT THOSE LINES TO ENABLE OR DISABLE TYPES OF CONNECTIONS
# Check https://proxycheck.io/api/#type_responses for all types of connections details
block_vpn: true # If true, the plugin will block VPN connections
block_openvpn: true # If true, the plugin will block OpenVPN connections
block_proxy: true # If true, the plugin will block Proxy connections
block_tor: true # If true, the plugin will block Tor connections
block_mobile: true # If true, the plugin will block Mobile connections
block_business: true # If true, the plugin will block Business connections
block_hosting: true # If true, the plugin will block hosting connections
```
## COMMON QUESTIONS
### How to get an API key?
You can get an API key from https://proxycheck.io/
### How to get the API URL?
The API URL is https://proxycheck.io/v2/
### Do you save data using this plugin?
No, we don't save any data. We only use the API to check if the IP is a VPN, OpenVPN, Proxy, Tor, Mobile, Business or Hosting connection.
### Will this plugin stay free?
Yes, this plugin will stay free forever. The only thing I ask is to give me credit if you use this plugin in your server.
The only thing you may pay for is the API key from proxycheck.io if the free one is not enough for you.
### How can I support you?
You can support me by giving me a star on GitHub and visiting my patrons page: https://www.patreon.com/yuri_hikari
