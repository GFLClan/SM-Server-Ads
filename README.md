# Server Ads
## Description
GFL's Server Ads plugin that prints global, game-specific, server-specific, and paid advertisements to all players on the server with an interval.

## Requirements
This plugin requires GFL's Core [plugin](https://github.com/GFLClan/SM-Core) and GFL's MySQL plugin to be added to the game server and enabled. Please ensure the MySQL database used for the GFL MySQL plugin has a table called `gfl_serverlist` where each server is stored.

## ConVars
* `sm_gflsa_ad_interval` => Interval in seconds to display an advertisement to chat (default `30`).
* `sm_gflsa_custom_ads_file` => The location to server-specific ads starting from `addons/sourcemod/configs` (default `customads.txt`).
* `sm_gflsa_global_tablename` => The table where all non-paid advertisements are stored (default `"gfl_adverts-default"`).
* `sm_gflsa_paid_tablename` => The table where all paid advertisements are stored (default `"gfl_adverts-paid"`).
* `sm_gflsa_game_id` => The game ID to pick game-specific advertisements from (default `4` for CS:GO).
* `sm_gflsa_db_priority` => Database priority to use for queries executed by the plugin (default `1`).
* `sm_gflsa_db_createtable` => If enabled, the plugin will attempt to create the paid and non-paid advertisement tables automatically if they do not exist (default `0`).
* `sm_gflsa_advancedebug` => Whether to enable verbose logging (default `0`).

## Credits
* [Christian Deacon](https://www.linkedin.com/in/christian-deacon-902042186/) - Creator