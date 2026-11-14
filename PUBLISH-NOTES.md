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
