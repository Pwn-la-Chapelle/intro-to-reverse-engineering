# En-Pawnssant

from **[Cyber Security Challenge Germany 2021 Qualifiers CTF](https://cscg.de)** (March 1 - June 1, 2021)

## Challenge

- **Category:** Reverse Engineering
- **Difficulty:** Hard
- **Author:** 0x4d5a

> Let's play a game of queens. No, a game of [pawns](https://www.compuphase.com/pawn/pawn.htm). I'll take en passant. No wait. I'm confused. All I know for sure is, that this Makefile was used:

```Makefile
PAWN := $(shell hexdump -n 4 -e '4/4 "%08X" 1 "\n"' /dev/random)
all:
    ./pawncc -k$(PAWN) crackme.p
```

**Files:**

- [`crackme.amx`](./crackme.amx)