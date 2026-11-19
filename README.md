# polytopia-matches

Finished Battle of Polytopia games fetched read-only from the game server, kept as training data for the Polytopia engine and AI.

## Layout
- `games/<first two characters of id>/<game id>/` holds one complete game:
  - `init.bin`: the starting state
  - `cur.bin`: the final state, with the full command history
  - `meta.json`: the server's wrapper for the game
- `lists/working_ids.txt`, `lists/working_links.txt`: ids that are still fetchable (bare ids and share links)
- `lists/dead_ids.tsv`: ids the server no longer has
- `lists/game_info.tsv`: mode, size, teams, turns, tribes and start date, where known
- `lists/SUMMARY.md`: counts

The game files are binary and are read by the `polyai-human` crate in the Polytopia repository.
