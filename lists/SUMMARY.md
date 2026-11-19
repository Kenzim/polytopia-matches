# Game id lists

- `working_ids.txt`, `working_links.txt`: 12401 ids that were fetchable from the game server when checked
- `dead_ids.tsv`: 1807 ids the server no longer had (`api:1005`, not found), with the error kind and message
- `game_info.tsv`: mode, map size, team count, turns, tribes and start date for the games where that is known

`games/` holds 12,436 complete games, which is every id in `working_ids.txt` plus 35 more.
