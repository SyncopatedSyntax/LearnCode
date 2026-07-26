# Linux Command Line Confidence — Resources

## Knowledge

- [Book: _The Linux Command Line_ — William Shotts](https://linuxcommand.org/tlcl.php)
  Free, complete beginner-to-intermediate book on the shell. Use for: foundational navigation, file operations, permissions, and how the shell actually works.
- [Pro Git — Scott Chacon & Ben Straub](https://git-scm.com/book/en/v2)
  The official free Git book. Use for: any git command from the terminal — commits, branches, remotes, GitHub workflows.
- [GitHub Docs](https://docs.github.com)
  Official GitHub documentation. Use for: what a GitHub-specific command or workflow (Actions, `gh` CLI, etc.) actually does.
- [Synology Knowledge Center — Terminal (DSM)](https://kb.synology.com/en-us/DSM/help/DSM/AdminCenter/system_terminal?version=7)
  Official Synology docs on the Control Panel Terminal & SNMP settings. Use for: anything about how SSH access is configured on the NAS itself.
- [explainshell.com](https://explainshell.com)
  Paste any shell command and it breaks down every flag and argument. Use for: decoding an unfamiliar command you found online before running it.
- [ss64.com/bash](https://ss64.com/bash/)
  Quick-reference command syntax pages. Use for: fast lookup of a command's flags once you know roughly what it does.

### Docker & YAML (NAS self-hosting)

- [Docker Compose file reference — official docs](https://docs.docker.com/reference/compose-file/)
  The authoritative spec for every key in a compose file. Use for: checking what a key actually does, and confirming whether syntax in a tutorial is current. Note it confirms the top-level `version:` key is obsolete.
- [Docker Compose — services reference](https://docs.docker.com/reference/compose-file/services/)
  The per-service keys: `image`, `ports`, `volumes`, `environment`, `restart`, `depends_on`. Use for: decoding a specific line in a compose file.
- [Container restart policies — Docker docs](https://docs.docker.com/engine/containers/start-containers-automatically/)
  Defines `no`, `always`, `on-failure`, `unless-stopped`. Use for: deciding what should happen after a NAS reboot.
- [yaml.org — official site](https://yaml.org/about/)
  The YAML spec and its origin. Use for: settling questions about YAML syntax itself, separate from Docker.
- [Synology Knowledge Center — Container Manager](https://kb.synology.com/en-us/DSM/help/ContainerManager/docker_desc?version=7)
  Official Synology docs for Container Manager (the renamed Docker package in DSM 7.2+), including its Project feature for compose files. Use for: anything NAS-specific about deploying containers.

## Wisdom (Communities)

- [r/linux4noobs](https://reddit.com/r/linux4noobs)
  Beginner-friendly, low judgment. Use for: "is this normal/safe" questions.
- [Synology Community Forum](https://community.synology.com)
  Official user forum. Use for: NAS-specific questions, especially before running anything unfamiliar via SSH on it.
- [Unix & Linux Stack Exchange](https://unix.stackexchange.com)
  Higher signal than general Stack Overflow for shell/OS questions. Use for: "why does this command do X" deep dives.
- [r/selfhosted](https://reddit.com/r/selfhosted)
  Large, active community running exactly the kind of containers you're aiming for. Use for: "is this app worth self-hosting", sanity-checking a compose file before you deploy it.

## Gaps
- No resource yet on the `gh` CLI (GitHub's official command-line tool) specifically — add once that becomes relevant.
- No vetted, high-trust source for *Synology-specific* compose recipes (PUID/PGID conventions, `/volume1/` path habits). Community blogs dominate this space and vary wildly in quality — treat any such tutorial with suspicion, especially if it still shows `version:` at the top, which dates it.
