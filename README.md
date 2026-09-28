# Gravis Ultrasound Game Patches

A collection of patches adding or improving **Gravis Ultrasound (GUS)** support in classic DOS games.

The idea behind the project is simple:

> **What if the Gravis Ultrasound had received more native game support?**

These patches explore that question by adapting games that are particularly well suited to the GUS — especially titles with tracker-based music, digital soundtracks, or audio engines that can benefit from the GUS hardware mixer.

The focus is on:

- Real DOS hardware
- GF1-compatible Gravis Ultrasound cards
- Low CPU overhead
- Hardware mixing where practical
- Good sound quality
- Configuration through the standard `ULTRASND` environment variable
- Simple installation
- Redistributable patches containing no original copyrighted game assets

## Downloads

| Game | GUS support | Repository | Download |
|---|---|---|---|
| **Prehistorik 2** | GUS music and sound effects | [prehistorik2-gus](https://github.com/koodoonas/prehistorik2-gus) | [Latest release](https://github.com/koodoonas/prehistorik2-gus/releases/latest) |
| **Disney's Aladdin** | GUS native support restored | [aladdin-gus](https://github.com/koodoonas/aladdin-gus) | [Latest release](https://github.com/koodoonas/aladdin-gus/releases/latest) |
| **Another World / Out of This World** | GUS audio with sample preloading | [another-world-gus](https://github.com/koodoonas/another-world-gus) | [Latest release](https://github.com/koodoonas/another-world-gus/releases/latest) |
| **James Pond 2: Codename RoboCod** | GUS music and sound effects | [james-pond-2-gus](https://github.com/koodoonas/james-pond-2-gus) | [Latest release](https://github.com/koodoonas/james-pond-2-gus/releases/latest) |
| **Cannon Fodder 2** | GUS music and sound effects | [cannon-fodder-2-gus](https://github.com/koodoonas/cannon-fodder-2-gus) | [Latest release](https://github.com/koodoonas/cannon-fodder-2-gus/releases/latest) |
| **Micro Machines 2** | GUS native HW mixing restored | (https://github.com/koodoonas/micro-machines-2-gus) | [Latest release](https://github.com/koodoonas/micro-machines-2-gus/releases/latest) |

More patches will be added as they become usable and are tested on real hardware.

## Hardware testing

Development and testing is primarily done on real DOS-era hardware rather than relying exclusively on emulation.

Current patches have been tested on systems including:

- **386DX-40 + Gravis Ultrasound MAX**
- **486DX4-133 + Gravis Ultrasound PnP**

Individual repositories contain more specific compatibility and configuration information.

## Configuration

Where possible, patches use the standard DOS Gravis Ultrasound environment variable:

```dos
SET ULTRASND=240,7,7,7,7
```

The exact values depend on your card configuration.

This avoids hard-coding one particular GUS setup and makes the patches usable across different systems and GUS-compatible cards.

See each project's README for its supported command-line options and installation procedure.

## Project goals

These are not attempts to rewrite the original games.

The goal is to create small, practical compatibility patches that make better use of Gravis Ultrasound hardware while preserving the original gameplay.

Priority is given to:

1. **Real hardware compatibility**
2. **Low CPU usage**, particularly on 386-class systems
3. **GUS hardware mixing** where the game architecture makes it practical
4. **High-quality playback**
5. **Minimal changes to the original game**
6. **No redistribution of original game assets**

## Why?

The Gravis Ultrasound was unusually capable hardware for its time, but relatively few DOS games took full advantage of it.

Its GF1 synthesizer could mix multiple sample voices in hardware, potentially reducing CPU load while providing tracker-style music and digital effects with excellent quality.

A large number of DOS games already contained the sort of sample-based music and audio assets that could have been a good match for the card.

These projects are an experiment in an alternate version of DOS gaming history:

**What might these games have sounded like if native GUS support had been more widespread?**

## Original games required

These repositories do **not** contain the original games.

You must supply your own copy of each supported game.

Unless explicitly documented otherwise, releases contain only original patch code, loaders, configuration utilities, documentation, and other redistributable project files.

## Compatibility

The primary target is genuine DOS hardware with a Gravis Ultrasound or compatible GF1 implementation.

Compatibility may vary depending on:

- GUS model
- DMA and IRQ configuration
- DOS memory configuration
- CPU speed
- Game version
- Sound card combinations
- Emulator accuracy

If you test a patch on hardware not already listed in its repository, compatibility reports are useful.

## Issues and testing

Please report problems in the **individual patch repository**, rather than this collection repository.

When reporting a hardware problem, include:

- CPU and system type
- GUS model
- `ULTRASND` setting
- DOS version
- Game version
- Other installed sound cards
- Memory manager configuration, if relevant
- Exact command line used

Real-hardware test results are especially useful.

## The collection

This repository acts as the index for the project.

Development, source code, documentation, issues, and releases remain in the individual game repositories:

- [Prehistorik 2 GUS](https://github.com/koodoonas/prehistorik2-gus)
- [Aladdin GUS](https://github.com/koodoonas/aladdin-gus)
- [Another World / Out of This World GUS](https://github.com/koodoonas/another-world-gus)
- [James Pond 2 GUS](https://github.com/koodoonas/james-pond-2-gus)
- [Cannon Fodder 2 GUS](https://github.com/koodoonas/cannon-fodder-2-gus)
- [Micro Machines 2](https://github.com/koodoonas/micro-machines-2-gus)

## Notable patches by others:
- [Xenon II — selectable Sound Blaster / Gravis UltraSound audio](https://github.com/pgeo101/xenon2-soundblaster)

## AI usage disclosure

These patches have been heavily assisted by AI and, in some cases, developed almost entirely with its help.

I remain ambivalent about AI and its human and environmental costs. But since it’s already here, I might as well use it for something fun until it consumes us all.

**Gravis Ultrasound lives.**
