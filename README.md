================================================================
KERNIMPLE
================================================================
An open source programming language designed for kernel development.
Simpler than C. More stable than Zig. Built for the bare metal.
================================================================


WHAT IS KERNIMPLE?
----------------------------------------------------------------
Kernimple is a programming language built specifically for kernel
and bare metal development. It is designed to be simpler than C,
more stable than Zig, and easier to learn — without losing the
low-level control that kernel development requires.

Kernimple has a built-in compiler. No separate toolchain download.
No configuration. Just write code and run it.


WHY KERNIMPLE?
----------------------------------------------------------------
Every existing kernel language has problems:

C       — powerful but hostile to beginners, no safety
Zig     — modern but unstable, changes between versions
Rust    — memory safe but extremely steep learning curve

Kernimple fixes this:

- Simple plain English syntax
- Built-in compiler, plug and run
- Stable — major updates every 9-10 months only
- Designed ONLY for kernel development, not general purpose
- Fully open source under GPL
- Complete documentation
- Community support


CURRENT STATUS
----------------------------------------------------------------
Kernimple is in early design/development stage.
Version 0.1 spec is complete and available in SPEC.txt.
The compiler is not yet built — contributions welcome.


WHAT IS IN THIS REPO
----------------------------------------------------------------
README.txt    — this file
SPEC.txt      — full Kernimple language specification v0.1
LICENSE       — GPL v3 open source license


QUICK LOOK AT KERNIMPLE SYNTAX
----------------------------------------------------------------
Here is a basic Kernimple kernel entry point:

    start {
        vprint(Kernimple booted)

        if/(detect h//screent=(oled)) {
            vprint(oled display detected)
        } else/(vprint(display detected))

        multime {
            vprint(kernel running)
        }
    }

Simple. Readable. No semicolons. No type declarations.
Anyone can look at that and understand what it does.


HOW TO CONTRIBUTE
----------------------------------------------------------------
Kernimple needs contributors to help build:

- The compiler (targets LLVM, C++ or C recommended)
- Standard library for kernel development
- Documentation and examples
- Testing and bug reports

To contribute:
1. Read the spec in SPEC.txt
2. Fork this repo
3. Make your changes
4. Submit a pull request
5. All changes must be open sourced under GPL


COMMUNITY
----------------------------------------------------------------
Discord and website coming soon.
For now open a GitHub issue to ask questions or share ideas.


LICENSE
----------------------------------------------------------------
Kernimple is licensed under the GNU General Public License v3.
See LICENSE file for full details.
Any modifications must also be open sourced under GPL.


================================================================
KERNIMPLE v0.1 — Built from scratch. For the bare metal.
================================================================
