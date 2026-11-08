**1. Download the kickoff kit:** [KIT LINK](https://drive.google.com/drive/folders/1Wn-ItiYiYT7ppuzeIhyaYWxSZdihaW8D?usp=drive_link)
It has the final problem statements (PDF) and one folder per problem with its interface files, public sample tests and harness. Start with `README.md`, then `00-Common/README.md`.

**2. Get the environment image** (Google Drive, about 3 GB; Problem 4 teams using FreeBSD, NetBSD, OpenBSD, 9front, Haiku or Redox also need `ostrack-full.tar.gz`): [DRIVE FOLDER LINK](https://drive.google.com/drive/folders/1vl6JkrfGxdbi6EyoW8yTeym8VOiFFLCz?usp=drive_link)

``` bash
docker load -i ostrack-core.tar.gz
docker run -it --rm --cap-add=SYS_PTRACE --security-opt seccomp=unconfined -v "$PWD":/work ostrack:core
```

Everything is offline and judged in this image. The kit is also inside it at `/opt/os-track/`.

**3. Pick one problem:** PageWeaver · ContextChaos · AnarchyOS · The Cat-V Minimalist Stack Challenge. Teams are ranked only against teams on the same problem.

Good luck, and have fun breaking things (deliberately)!
