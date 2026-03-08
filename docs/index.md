<!--| [Repository](https://github.com/RedPepperDec/RedPepper) | [Discord](https://discord.gg/RazNaFGXfG) |
|----------------------------------------------------------|------------------------------------------------------------|------------------------------------------|
-->
# Project RedPepper

[*View project*](https://github.com/RedPepperDec/RedPepper)<br>  

An in-progress decompilation of [*Super Mario 3D Land*](https://wikipedia.org/wiki/Super_Mario_3D_Land) for the [*Nintendo 3DS*](https://wikipedia.org/wiki/Nintendo_3DS).  
The focus is currently laid on the European release, but multiversion groundwork was made for all [available versions](#versions).  
  
There are no known symbol maps for this game, however, you can use affiliated games, such as:  

- Super Mario Galaxy: The game was based on SMG2, and while we dont have its symbol map, we have that of SMG1. It was put into al::
- Captain Toad Treasure Tracker (SW): Switch version provides symbols, while the direct 3DS version does not.
- Super Mario 3D World (SW): It is a mix of Super Mario Odyssey and Super Mario 3D World, which came after 3DL.
- Super Mario Odyssey: Has a full function map, including private functions.
- SEAD: explore [debugging.games](https://debugging.games/3DS) for 3DS games with SEAD (MK7,Nintendogs,Zelda Tri-Force at Unmatched/3DS) or just use PEAD from [libpia_pead.a](https://debugging.games/_files/Other/Nintendo%20EAD%20Standard%20Library/[3DS]%20Nintendo%20EAD%20Standard%20Library%20(P2P%20+%20Pia%20Port%20+%20Rewrite)%20(DWARF+SYMTAB)%20[2014-09-17].7z)


Code Variants
---
| Region | Variant | Started? | Release Date |  CTR-SDK  | sha256sum                                                        |
|--------|---------|----------|--------------|-----------|------------------------------------------------------------------|
| Europe | Release |    Yes   | Nov. 18 2011 | 2.4.1.200 | e1d7e188ff88467df776c17cec45c44857fadf5b699944baa8cddcae7d939e64 |
| Europe | Kiosk   |     No   | Unknown      | 2.4.1.200 | 184b8804ccf4aea9f447b2278dfc3171d4f8c4e6abf890d7b24680d649e034c6 |
| Japan  | Release |     No   | Nov. 3 2011  | 2.4.1.200 | 885dcaed5994076732b1f99e452a6f06493c23464ae0509ebbf44b8c6fd614a7 |
| Japan  | Kiosk   |     No   | Unknown      | 2.4.1.200 | b1987a589ddb9d4caf723e0dfb470131d2aee52023b8b9a90455f6c9f694fefc |
|  USA   | Release |     No   | Nov. 13 2011 | 2.4.1.200 | c705711154b1c514d7a0b5d133fabff42834110b198bd4cf86397d0d1c1597e9 |
|  USA   | E3 Demo |     No   | Unknown      | 2.3.2.200 | 6016cbdada120b2476e512e8c87c5d525f62ee8daa9f81e00c8caa1237477344 |
| China  | Release |     No   | Dec. 7 2012  | 3.3.0.200 | 11ca2f6fa7e8b9553737830899787e7236f4fdbf8b96ed03c99fbe6a8939b37d |
| Taiwan | Release |     No   | Dec. 7 2012  | 3.3.0.200 | 6207415ee0c6d2dff53d65b39cc2b05318a3b25e62e39639ab2a7243d96357f0 |
| Korea  | Release |     No   | Apr. 28 2012 | 3.3.0.200 | 820940dc19b86f8d47515973d9f1484c4efc0571a729c294e85b53e5097fda56 |

Libraries
---
- AL
- SEAD
    - NintendoWare
    - MessageSystem
    - CTR SDK

External resources
---
- [Original repo](https://github.com/3dsdecomp/RedPepper)
- [3D Mario Decompilation Discord](https://discord.gg/RazNaFGXfG)

~Moddimation
