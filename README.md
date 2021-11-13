# GhidraBoy source for reference

https://github.com/Gekkio/GhidraBoy

------------------------------------------------------------------------------
## Features

* Sharp SM83 (CPU core used in Game Boy) support for Sleigh
* Game Boy ROM loader:
  - Can load unbanked ROMs (&lt;= 32kB, e.g. Tetris)
  - Can load banked ROMs (&gt; >32kB, e.g. Pokemon)
  - Can load greyscale boot ROMs (DMG/DMG0/MGB/SGB/SGB2)
  - Can load color boot ROMs (CGB/CGB0)
* Memory blocks based on the hardware memory map
  - Banked regions use overlays (TODO: figure out if there's a better way to
    support them)
  - GB vs GBC differences are handled (e.g. banked WRAM)
- Symbols for hardware registers (0xFFxx range)
  - GB vs GBC differences are handled (e.g. existence of KEY1 register)
* Game Boy cartridge header data types
  - Enumerated types for some things
