# Mission: Linux Command Line Confidence

## Why
You want to stop feeling intimidated by any Linux terminal you run into. Right now that shows up in three places you actually touch: working with GitHub from the command line, navigating a Linux file system, and SSH'ing into your Synology NAS. This mission is about the underlying skill — comfort with the terminal in general — not memorizing three separate command lists.

## Success looks like
- You can look at an unfamiliar terminal command and figure out roughly what it does before running it (or know how to check, e.g. `man`, `--help`, explainshell.com).
- You can navigate any Linux file system confidently: know where you are, move around, find things, read files, without needing a GUI.
- You can SSH into your Synology NAS, look around, and check on things without fear of breaking it.
- You can use Git from the terminal for your own repos instead of defaulting to the GitHub website.
- You can read a `docker-compose.yml` line by line and know what each part does, instead of pasting one from a tutorial and hoping — so you can self-host apps on the NAS deliberately.

## Constraints
- Beginner — assume no prior command-line experience.
- Caution around the Synology NAS specifically: you have working SSH access but do not want to risk breaking it. Early NAS-touching exercises stick to read-only, non-destructive commands, and anything with real risk (deleting, moving, permissions, package/system changes) gets called out explicitly before use.

## Out of scope
- Deep Linux system administration on the NAS (DSM internals, reconfiguring system services) — general confidence and safe navigation only.
- Docker beyond self-hosting on the NAS: building your own images, Dockerfiles, multi-stage builds, orchestration (Swarm/Kubernetes). The goal is confidently *using* other people's containers, not authoring them.

_Scope note (July 2026): expanded to include reading and writing Docker Compose files for NAS self-hosting — see [[0004-mission-expanded-to-docker-on-nas]]._
