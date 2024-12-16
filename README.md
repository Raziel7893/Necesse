# WindowsGSM.Necesse
🧩WindowsGSM plugin that provides Necesse Dedicated server

## PLEASE ⭐STAR⭐ THE REPO IF YOU LIKE IT! THANKS!

### Notes
- If local connections work but not External: see chapter Portforwarding
- IP needs to be your local one (like in almost every WGSM server)
- The ServerMap field will be used for choosing your world/savegame
- If you change the datadir value, you will need to start the Server once without the -nogui parameter to setup the world and initial config.

### WindowsGSM Installation: 
1. Download  WindowsGSM https://windowsgsm.com/ 
2. Create a Folder at a Location you wan't all Server to be Installed and Run.
3. Drag WindowsGSM.Exe into previously created folder and execute it.

### Plugin Installation:
1. Download [latest](https://https://github.com/Raziel7893/WindowsGSM.Necesse/releases/latest) release
2. Either Extract then Move the folder **Necesse.cs** to **WindowsGSM/plugins** 
    1. Press on the Puzzle Icon in the left bottom side and press **[RELOAD PLUGINS]** or restart WindowsGSM
3. Or Press on the Puzzle Icon in the left bottom side and press **[IMPORT PLUGIN]** and choose the downloaded .zip

### Official Documentation
🗃️ https://necessewiki.com/Multiplayer

### The Game
🕹️ https://store.steampowered.com/app/1169040/Necesse/

### Dedicated server info
🖥️ https://steamdb.info/app/1169370/info/

### Port Forwarding (YOU NEED THIS, TO BE ABLE TO CONNECT FROM THE INTERNET(only for servers/pcs at home):
- If You don't know How: portforward.com
- 14159 UDP - Default Game Port

### Files To Backup
- Save Gane (You could only save serverfiles/Necesse/Saved , but that includes many big logs)
  - %appdata%/Necesse/Saved/SaveGames/cfg
  - %appdata%/Necesse/Saved/SaveGames/saves
  - WindowsGSM\servers\%ID%\configs

### Available Params
settings are in %appdata%\Necesse\cfg.
Activly applied Wgsm Configs (those will most likely overwrite whats in the cfg):
- Server Start Param		//passed to serverexecutable
- Server Map				//used to choose which world/savegame is used
- Server Port				//Port the server is started on
- Server MaxPlayers			//maximum allowed players
All other parameters in WGSM are ignored completly.

### Not having an full IPv4 adress ( named CCNAT or DSL Light )
No game or gameserver supports ipv6 only connections. 
- You need to either buy one (most VPN services provide that option. A pal uses ovpn.net for his server, I know of nordvpn also providing that. Should both cost around 7€ cheaper half of it, if your already having an VPN)
- Or you pay a bit more for your internet and take a contract with full ipv4. (depending on your country)
- There are also tunneling methods, which require acces to a server with a full ipv4. Some small VPS can be obtained, not powerfull enough for the servers themself, but only for forwarding. I think there are some for under 5€), the connection is then done via wireguard. but its a bit configuration heavy to setup) 

Or you connect your friends via VPN to your net and play via local lan then.
Many windowsgsm plugin creators recommend zerotier (should be a free VPN designated for gaming) , see chapter below (or tailscale, but no howto there)

## How can you play with your friends without port forwarding?
- Use [zerotier](https://www.zerotier.com/) folow the basic guide and create network
- Download the client app and join to your network
- Create static IP address for your host machine
- Edit WGSM IP Address to your recently created static IP address
- Give your network ID to your friends
- After they've joined to your network
- They can connect using the IP you've created eg: 10.123.17.1:7777
- Enjoy

### Support
[WGSM](https://discord.com/channels/590590698907107340/645730252672335893)

### Give Love!
[Buy me a coffee](https://ko-fi.com/raziel7893)

[Paypal](https://paypal.me/raziel7893)

### License
This project is licensed under the MIT License - see the <a href="https://github.com/raziel7893/WindowsGSM.Necesse/blob/main/LICENSE">LICENSE.md</a> file for details

### Thanks
Thanks to ohmcodes for the Enshrouded and Palworld Plugins which i used for guidance to create this one
