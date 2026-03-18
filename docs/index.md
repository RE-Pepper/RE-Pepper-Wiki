# {{ config.project_name }}

Links: [**Github**](https://github.com/RE-Pepper/RE-Pepper)  
Discord: [**3DL Decomp**](https://discord.gg/wK4ZKa9QXq) | [**3DS Decomp**](https://discord.gg/wK4ZKa9QXq) | [**3DL Modding (old)**](https://discord.gg/kjJwaTCQRe) | [**3DL Modding (new)**](https://discord.gg/9FEhR5kCJc)  

This is RE:Pepper, an abbrevation for *Reverse Engineering *[***Super Mario 3D Land***](https://wikipedia.org/wiki/Super_Mario_3D_Land) Project for the [*Nintendo 3DS*](https://wikipedia.org/wiki/Nintendo_3DS).  
The focus is currently laid on the European release, but the repo has experimental multi-version support for all [available versions](#versions).  
  
There are no known symbol maps for this game, however, you can use affiliated games, such as:  

- Super Mario Odyssey: Has a full function map, including private functions.
- Super Mario Galaxy: The game was based on SMG2, and while we dont have its symbol map, we have that of SMG1. It was put into al::
- Captain Toad Treasure Tracker (SW): Game is partly based on 3D World, and the Switch version provides symbols, while the direct 3DS version does not.
- Super Mario 3D World - Bowsers Fury (SW): It is a mix of Super Mario Odyssey and Super Mario 3D World, which came after 3DL.
- SEAD: explore [debugging.games](https://debugging.games/3DS) for 3DS games with SEAD/PEAD (MK7,Nintendogs,Zelda at 3DS or Tri-Force at Unmatched/3DS)
  
Note: I fixed the map for tri-force, which has sead debug. For that, msg me on discord (moddimation)  
Note: RedPepper is the internal codename for Super Mario 3D Land.  

Code Variants
---
| Region | Variant | Started? | Release Date |  CTR-SDK  | sha256sum                                                        |
|--------|---------|----------|--------------|-----------|------------------------------------------------------------------|
| Europe | Release |    Yes   | Nov. 18 2011 | 2.4.1.200 | e1d7e188ff88467df776c17cec45c44857fadf5b699944baa8cddcae7d939e64 |
|  USA   | Release |     No   | Nov. 13 2011 | 2.4.1.200 | c705711154b1c514d7a0b5d133fabff42834110b198bd4cf86397d0d1c1597e9 |
| Japan  | Release |     No   | Nov. 3 2011  | 2.4.1.200 | 885dcaed5994076732b1f99e452a6f06493c23464ae0509ebbf44b8c6fd614a7 |
| Europe | Kiosk   |     No   | Unknown      | 2.4.1.200 | 184b8804ccf4aea9f447b2278dfc3171d4f8c4e6abf890d7b24680d649e034c6 |
| Japan  | Kiosk   |     No   | Unknown      | 2.4.1.200 | b1987a589ddb9d4caf723e0dfb470131d2aee52023b8b9a90455f6c9f694fefc |
|  USA   | E3 Demo |     No   | Unknown      | 2.3.2.200 | 6016cbdada120b2476e512e8c87c5d525f62ee8daa9f81e00c8caa1237477344 |
| Taiwan | Release |     No   | Dec. 7 2012  | 3.3.0.200 | 6207415ee0c6d2dff53d65b39cc2b05318a3b25e62e39639ab2a7243d96357f0 |
| Korea  | Release |     No   | Apr. 28 2012 | 3.3.0.200 | 820940dc19b86f8d47515973d9f1484c4efc0571a729c294e85b53e5097fda56 |
| China  | Release |     No   | Dec. 7 2012  | 3.3.0.200 | 11ca2f6fa7e8b9553737830899787e7236f4fdbf8b96ed03c99fbe6a8939b37d |

Libraries
---
- AL
- SEAD
    - MessageSystem
- NintendoWare
- CTR SDK

External resources
---
- [Original Project](https://github.com/3dsdecomp/RedPepper)
- [SEAD reference from open-ead](https://github.com/open-ead/sead)
- [SEAD reference from stupidestmodder](https://github.com/stupidestmodder/sead-fork)

~Moddimation
