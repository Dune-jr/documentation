# Server Settings

There are lots of server settings to change all from the score limit, to the speed of the shotgun. This doc will show you what those are, not how to set up a server. Read the [Server Setup](server_setup.md) doc to learn that. For server commands, see the [Server Commands](server_commands.md) doc.

**Syntax:** setting value

### Physics settings

To change the game's physics, read the [Server Tuning](server_tuning.md) doc.

### Engine settings

`*` means it can't be changed while running the server.

|Settings|	Description|	Default|
| ------ | ---------- | -------- |
|`sv_name` |	Name of the server|	unnamed server|
|`bindaddr` *|	Address to bind	| |
|`sv_port` *|	Port the server will listen on|	8303|
|`sv_external_port` *|	Port to report to the master servers (e.g. in case of a firewall rename)|	0|
|`sv_max_clients` *|	Number of clients that can be connected to the server at the same time|	12|
|`sv_max_clients_per_ip`|	Number of clients with the same ip that can be connected to the server at the same time|	12|
|`sv_high_bandwidth` *|	Use high bandwidth mode, for LAN servers only|	0|
|`sv_register`|	Register on the master servers|	1|
|`sv_map`|	Map to use|	dm1|
|`sv_rcon_password`|	Password to access the remote console (if not set, rcon is disabled)|  |
|`password`|	Password to connect to the server|	|
|`logfile`|	Path to a logfile| |
|`console_output_level`|	Adjust the amount of messages in the console|	0|
|`sv_rcon_max_tries`|	Maximum number of tries for remote console authetication|	3|
|`sv_rcon_bantime`|	Time (in minutes) a client gets banned if remote console authentication fails (0 makes it just use kick)|	5|
|`sv_auto_demo_record`| Automatically record demos| 0|
|`sv_auto_demo_max`| Maximum number of automatically recorded demos (0 = no limit)| 10|
|`ec_bindaddr`|Address to bind the external console to. Anything but 'localhost' is dangerous"|localhost|
|`ec_port`|Port to use for the external console||
|`ec_password`|External console password"||
|`ec_bantime`|The time a client gets banned if econ authentication fails. 0 just closes the connection|0|
|`ec_auth_timeout`|Time in seconds before the the econ authentication times out|30|
|`ec_output_level`|Adjusts the amount of information in the external console|1|

### Game settings

|Settings|	Description|	Default|
| ------ | ---------- | -------- |
|`sv_warmup`|	Warmup time between rounds|	0|
|`sv_scorelimit`|	Score limit of the game (0 disables it)|	20|
|`sv_timelimit`|	Time limit of the game (in case of equal points there will be sudden death)|	0|
|`sv_gametype`|	Gametype (dm/ctf/tdm) (This setting needs the map to be reloaded in order to take effect)|	dm|
|`sv_maprotation`|	The maps to be rotated|	|
|`sv_rounds_per_map`|	Number of rounds before changing to next map in rotation|	1|
|`sv_motd`|	Message of the day, shown in server info and when joining a server|	|
|`sv_spectator_slots`|	Number of clients that can only be spectators|	0|
|`sv_teambalance_time`|	Time in minutes after the teams are uneven, to auto balance|	1|
|`sv_spamprotection`|	Enable spam filter|	1|
|`sv_tournament_mode`|	Players will automatically join as spectator|	0|
|`sv_respawn_delay_tdm`|	Time in seconds needed to respawn in the tdm gametype|	3|
|`sv_teamdamage`|	Enable friendly fire|	0|
|`sv_powerups`|	Enable powerups (katana)|	1|
|`sv_vote_kick`|	Enable kick voting|	1|
|`sv_vote_kick_bantime`|	Time in minutes to ban a player if kicked by voting (0 equals only kick)|	5|
|`sv_vote_kick_min`|	Minimum number of players required to start a kick vote|	0|
|`sv_inactivekick_time`|	Time in minutes after an inactive player will be taken care of|	3|
|`sv_inactivekick`|	How to deal with inactive players (0 = move to spectator, 1 = move to free spectator slot/kick, 2 = kick)|	1|
