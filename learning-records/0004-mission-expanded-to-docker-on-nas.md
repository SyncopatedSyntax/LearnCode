# Mission expanded: Docker Compose for self-hosting on the NAS

The user asked to learn YAML in Docker, with the stated driver being **running apps on their Synology NAS**. This extends [[MISSION]] beyond the original Linux-commands scope — which had anticipated exactly this, listing NAS deep-dives as out of scope "unless you ask to go further later."

**Prior knowledge disclosed:** they have already run containers by copying `docker-compose` files from tutorials and getting them working, but do not understand what the individual lines do. So this is *not* a from-zero container topic — the right entry point is decoding a file they can already make work, not explaining what a container is.

**Implication:** teach compose files as a reading-comprehension skill first (decode → then modify → then write). Their existing copied files are the practice material. Note also that tutorials they copied from are likely outdated — the top-level `version:` key is now obsolete in the Compose Specification, which is a probable misconception to correct early.
