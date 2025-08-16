
## Minecraft V1.2.5 private server ##
EDIT:Hey so to actually have other people join use Radmin VPN 
i've put it there for you then once its setup click: "network"  
then: "Create network" then make a network and make a password 
then BOOM under Desktop or what ever you have your laptop/PC 
named as you'll see something like this eg: 26.157.52.193
then your friends use that as a address on minecraft and now PLAY!

DM me on discord for help: Kiyoshi_brits


To change any settings, edit server.properties.

To start the server, run "start server.bat" on windows.

Add any user names you want to have op to ops.txt

Ingame, ops can use the following commands:
kick <player>             removes a player from the server
   
ban <player>              bans a player from the server

pardon <player>           pardons a banned player so that they can connect again

ban-ip <ip>               bans an IP address from the server

pardon-ip <ip>            pardons a banned IP address so that they can connect again

op <player>               turns a player into an op

deop <player>             removes op status from a player

tp <player1> <player2>    moves one player to the same location as another player

give <player> <id> [num]  gives a player a resource

tell <player> <message>   sends a private message to a player

stop                      gracefully stops the server

save-all                  forces a server-wide level save

save-off                  disables terrain saving (useful for backup scripts)

list                      lists all currently connected players

say <message>             broadcasts a message to all players

time <add|set> <amount>   adds to or sets the world time (0-24000)

gamemode <player> <mode>  sets player's game mode 0 or 1 (0=survival 1=creative)

toggledownfall            toggles rain on or off

xp <player> <amount>      gives the player the amount of xp (0-5000)



## Changelog:
Version 1.11:

+No more unbreakable blocks, MAKES NO SENSE

Version 1.10.1:

+ Fixed grow-trees again

Version 1.10:

+ Added a HUGE warning for running without verify-names turned off
+ Fixed grow-trees
+ Fixed a bug where people with long usernames could connect
+ Added admin-slot to server.properties. Setting this to true prevents people from logging in if the server is almost full and they're not admins.

Version 1.9.1:

+ Made tree growing a server option (grow-trees)
+ Opping or de-opping a user now updates their client without forcing them to log out/in

Version 1.9:

+ Added support for new tile types.
+ Fixed exploit where someone logging in with an illegal name would cause players to disconnect.

Version 1.8.2:

+ Ooops, everyone could build unbreakable blocks! Fixed!

Version 1.8.1:

+ Fixed a protocol error.

Version 1.8:

+ Added a whole bunch of new tile types
+ Players can no longer destroy unbreakable stone. Admins can, though!
+ Added /solid command to toggle stone tile type between normal and unbreakable

Version 1.7:

+ Added /tp as an alias for teleport

Version 1.6:

+ Fixed sponge working weirdly

Version 1.5:

+ Fixed a client crash bug on chat
+ You can now send most admin commands via stdin
+ Added chat throttling. Players who spam the chat will get muted for eight seconds
+ Added movement throttling. The server will not process more than a single move command per tick.
  (stand still to catch up if you're lagging)
+ Added max-connections to server.properties. This is the maximum number of connections per ip to the server. Default is three. 

Version 1.4.1:

+ Fixed bad names connecting and crashing all players

Version 1.4:

+ Added a /teleport command. It doesn't work yet, though, since it requires a client update.
+ Tried to fix two remove client crashes

Version 1.3:

+ Name security
+ Server-side client verification
+ Add logged-in.txt on the server
+ added /setspawn command for admins
+ Fix heartbeat pausing the game
+ Don’t let people spam ping requests
+ Fix ban ip (it was working, but not intuitive)
+ Various server fill exploit preventions. No more lava floods!
+ Private server adresses changed behavior, sorry. The server generates an externalurl.txt when run now.
+ Added verify-names to properties. Set this to false to allow people to connect directly via http://www.minecraft.net/play.jsp?ip=<ip>&port=<port>

Version 1.2:

+ Fixed a connection problem
+ Maybe fixed /banip

Version 1.1:

+ Made the private flag work
+ Added a /say command. Used to be /broadcast

Version 1.0:

  Initial release
