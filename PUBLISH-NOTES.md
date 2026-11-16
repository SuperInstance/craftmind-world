# craftmind-world — publish notes (2026-11-14)

The Craftmind League world save, copied read-only from the live server
directory on the Orin (~/minecraft-server) at programme rest.

## Contents
- `world/` — the league world: Cody's home district, the bowl, the
  day-18 stair, playerdata, advancements and stats.
- `world-26.3-backup/` — an earlier full backup of the world (26.3 era).
- `config/` — Paper global/world-defaults YAML.
- Root server text configs: bukkit.yml, spigot.yml, commands.yml,
  help.yml, permissions.yml, ops.json, whitelist.json, ban lists,
  usercache.json, eula.txt, version_history.json.

## Withheld / excluded (still on the Orin, deliberately not published)
- `server.properties` — EXCLUDED-SECRET: contains live credential
  fields (management-server-secret, management-server-tls-keystore-
  password). Values never copied here.
- Server runtime (re-downloadable): paper jars, libraries/, versions/,
  cache/.
- logs/ and plugins/ (bStats + spark data dirs) — server ephemera.
- session.lock files — runtime artefacts of the copy moment.

## Final snapshot — 2026-11-16

Programme shutdown (Casey's order, 2026-11-16). The Paper server
was stopped gracefully via its systemd user unit at 16:35:59 UTC
(log: Stopping server -> Saving players -> Saving worlds ->
ThreadedAnvilChunkStorage: All dimensions are saved), the unit was
disabled, and this commit is the world exactly as saved at that
stop. The local server directory was then pruned; revival
instructions are in SHUTDOWN-20261116.md in
SuperInstance/craftmind-league. server.properties remains withheld
(live credentials) and is preserved in the Thor away archive.
