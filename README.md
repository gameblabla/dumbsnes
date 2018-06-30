# DumbSNES

Primitive emulator based on PocketSNES 1.39 with some backport from PocketSNES 1.43 and Snes9x 2002.
The goal of this emulator is to be fast and run on resource-contrained platforms like the RS-97.

If your hardware is more capable then check out PocketSNES based on Snes9x 1.43 by Nebuleon instead.

On the RS-97, DumbSNES is provided into two executables : 

One without transparency which is faster but has some issues with games like Link to the Past, Super Metroid and Super Mario World.
The non-transpanrecy version is also more compatible and less glitchy with games like Uniracers.

The other one, the one with transparency, fixes more issues on Link, Metroid & Mario but is slower.
In the latter's case, it is advised to overclock to 600Mhz and even beyond if needed.

Detection is done with an sh script, if a game is blacklisted, it will run the transparency version instead.
If not, it defaults back to the non-transparent version.

# Issues

SuperFX support was removed because it was fairly broken on Snes9x.

This could eventually be fixed in a later version (and seperated like the 2 versions we have rn).

# License

Snes9x is, of course, non-commercial only. Pretty much the only alternative that is decent

and under the GPL is an old version of Mednafen, which was based on bsnes 0.59.

Too bad that even that version is pretty slow. (20 FPS on the GCW0)
