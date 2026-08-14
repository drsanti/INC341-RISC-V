# Assembly examples (`asm/`)

These `.s` files are the code used with the [course playlist](https://www.youtube.com/playlist?list=PLBPFpqyTjzeU8jpwZz2wLRCzuLZBm3LkM). Open them in the class IDE (VS Code + Venus) as shown in EP01–EP02.

| File | Related video(s) | Topics |
|------|------------------|--------|
| `asm01.s` | EP02 | Minimal / starter file for a new project |
| `asm02.s` | EP07 (demo) | Venus `ecall` I/O: pixels, LED row, 7-seg, buttons |
| `asm03.s` | EP03 | Registers, privilege notes, register aliases |
| `asm04.s` | EP04 | `li`, `mv` — immediates and register-to-register |
| `asm05.s` | EP05 | Pseudo-instructions vs standard instructions |
| `asm06.s` | EP06 | Directives (`.text`, `.globl`), delay, LED RGB test |
| `asm07.s` | EP07 | Environment call — set pixel |
| `asm08.s` | EP08 | Functions: `jal` / `jalr`, labels, `.text` / `.globl` |
| `asm09.s` | EP09 | Print int/hex/char/string, exit; simple `add` helper |
| `asm10.s` | EP10 | LED control via `ecall` |
| `asm11.s` | EP11 | Conditional branch (`blt`), true/false paths |
| `asm12.s` | EP12 | Branch / loop skeleton (pair with `resources/c12.c`) |
| `asm13.s` | EP13 | Delay subroutine, blinking LEDs / state patterns |
| `asm14.s` | EP14 | 7-segment digit codes, lookup table, `get_code` |
| `asm15.s` | EP15 | 7-segment + delay / counter patterns |
| `asm16.s` | EP15 (extended) | Larger 7-segment / counter lab program |
| `test.s` | — | Scratch / memory-segment notes for experiments |

## C companions in `resources/`

| File | Pair with | Purpose |
|------|-----------|---------|
| [`../resources/c08.c`](../resources/c08.c) | EP08 / `asm08.s` | Functions in C (`plus3`, `add`) vs ASM calling convention |
| [`../resources/c12.c`](../resources/c12.c) | EP12 / `asm12.s` | `if` / `for` / `while` / `do-while` structures to map to branches |

## Diagrams

Flowcharts for LED / control-flow labs:

- [`../resources/diagrams/flowcharts.drawio`](../resources/diagrams/flowcharts.drawio)
- [`../resources/diagrams/diagram.drawio`](../resources/diagrams/diagram.drawio)

Open with [diagrams.net](https://app.diagrams.net/) (draw.io).

## Suggested study order

1. EP01–EP05 → `asm01` … `asm05` (Quiz 2)  
2. EP06–EP09 → `asm06` … `asm09` + `c08.c` (Quiz 3)  
3. EP10–EP15 → `asm10` … `asm16` + `c12.c` + diagrams (Quiz 4)  
