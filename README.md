# INC341 — Embedded System I (RISC-V ASM)

Course materials and lab examples for **Embedded System I**, focused on computer fundamentals and **RISC-V assembly language programming**.

**Playlist:** [Embedded System I (RISC-V ASM)](https://www.youtube.com/playlist?list=PLBPFpqyTjzeU8jpwZz2wLRCzuLZBm3LkM)  
**Repository:** [github.com/drsanti/INC341-RISC-V](https://github.com/drsanti/INC341-RISC-V)

![VS Code / Venus IDE](resources/images/vscode-window.png)

## Table of contents

- [Course structure](#course-structure)
- [Assessment (2026)](#assessment-2026)
  - [Study checklist by quiz](#study-checklist-by-quiz)
- [Repository layout](#repository-layout)
- [Getting started](#getting-started)
- [Related links](#related-links)

---

## Course structure

| Phase  | Videos                                                                                                            | Focus                                               |
| ------ | ----------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| Basics | [BASIC-00](https://www.youtube.com/watch?v=h1wFicWQ6Nk) … [BASIC-07](https://www.youtube.com/watch?v=SW5j-7FS-qA) | Computers, architecture, buses, memory, ISA         |
| Labs   | [EP01](https://www.youtube.com/watch?v=BAjiCSVM9pQ) … [EP15](https://www.youtube.com/watch?v=bs63SiqeM4o)         | Tools, RISC-V ASM, debugging, I/O (LEDs, 7-segment) |

Full video index (titles, durations, links): [docs/PLAYLIST.md](docs/PLAYLIST.md)

---

## Assessment (2026)

**All quizzes:** Time **13:30–14:30** · Room **CB40610**

| Quiz       | Date              | Study scope         | Weight  | Theory | Programming |
| ---------- | ----------------- | ------------------- | ------- | ------ | ----------- |
| **Quiz 1** | 1 September 2026  | BASIC-01 → BASIC-07 | **20%** | 20%    | —           |
| **Quiz 2** | 22 September 2026 | EP01 → EP05         | **20%** | 15%    | 5%          |
| **Quiz 3** | 20 October 2026   | EP06 → EP09         | **25%** | 15%    | 10%         |
| **Quiz 4** | 17 November 2026  | EP10 → EP15         | **35%** | 25%    | 10%         |

**Total: 100%** (theory 75%, programming 25%)

### Study checklist by quiz

**Quiz 1 — theory only**

- BASIC-01 Introduction to Computer
- BASIC-02 Computer Architecture
- BASIC-03 System Buses
- BASIC-04 Data and Memory
- BASIC-05 Address Decoder
- BASIC-06 CPU Families and Instruction Set Architectures (ISA)
- BASIC-07 Embedded System RISC-V ISA and Assembly Language

_(BASIC-00 is course overview; recommended before Quiz 1, not listed in the quiz scope above.)_

Practice set (ตัวอย่างแนวข้อสอบ + เฉลย): [`docs/quizes/quiz1_example_computer_architecture.md`](docs/quizes/quiz1_example_computer_architecture.md)

**Quiz 2 — tools & first instructions**

- EP01 Software Tools Installation
- EP02 Create a New Project
- EP03 Registers and Alias Registers
- EP04 Load Immediate & Register-to-Register Transfer
- EP05 Pseudo Instructions and Standard Instructions

**Quiz 3 — debug, ecall, functions**

- EP06 Debugger Settings and Debugging Tools
- EP07 Environment Call
- EP08 Function
- EP09 Print and Exit Functions

> **Bonus (+2):** Handwritten notes on **2 pages of A4 paper** earn a special **+2** bonus.

**Quiz 4 — control flow & peripherals**

- EP10 LEDs Control (+ flowchart & diagram)
- EP11 Conditional Branch / Jump
- EP12 Conditional Branch and Loop Operations
- EP13 Delay and Blinking LEDs
- EP14 7-Segment Display Codes
- EP15 7-Segment and Counter

---

## Repository layout

```
INC341-RISC-V/
├── README.md                 # This file
├── docs/
│   ├── PLAYLIST.md           # Full YouTube playlist index
│   └── quizes/               # Quiz practice sets & answer keys
├── asm/                      # Assembly examples used in the videos
│   ├── README.md             # File ↔ episode mapping
│   ├── asm01.s … asm16.s
│   └── test.s
├── resources/                # Supporting C snippets, diagrams, images
│   ├── c08.c, c12.c          # C parallels for EP08 / EP12
│   ├── diagrams/             # draw.io flowcharts
│   └── images/
└── .vscode/                  # Venus / editor settings for the lab IDE
```

| Path                                   | Contents                                                                                       |
| -------------------------------------- | ---------------------------------------------------------------------------------------------- |
| [`asm/`](asm/)                         | RISC-V assembly examples demonstrated in the playlist                                          |
| [`resources/`](resources/)             | C reference snippets, draw.io diagrams, screenshots                                            |
| [`docs/PLAYLIST.md`](docs/PLAYLIST.md) | Complete video list with links and durations                                                   |
| [`docs/quizes/`](docs/quizes/)         | Quiz practice sets (e.g. [Quiz 1 example](docs/quizes/quiz1_example_computer_architecture.md)) |
| [`.vscode/`](.vscode/)                 | Workspace settings (Venus variable format, theme, etc.)                                        |

---

## Getting started

1. Watch **BASIC-00** and install tools as shown in **EP01**.
2. Create/open a project as in **EP02** (VS Code + [Venus](https://marketplace.visualstudio.com/items?itemName=hm.riscv-venus) or equivalent RISC-V ASM workflow used in class).
3. Work through examples in [`asm/`](asm/) in playlist order — see [`asm/README.md`](asm/README.md).
4. Use [`resources/`](resources/) for C comparisons and diagrams when studying functions and control flow.

---

## Related links

- Playlist: https://www.youtube.com/playlist?list=PLBPFpqyTjzeU8jpwZz2wLRCzuLZBm3LkM
- Older companion notes (registers / examples): https://github.com/drsanti/risc-v-assembly-programming
