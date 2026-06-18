# K1SS

Open source modular musical instruments.  
Assembled in Franche-Comté, France.

**Hardware:** [CERN-OHL-S 2.0](LICENSE_HARDWARE) · **Firmware:** GPL-3.0 · **Documentation:** CC-BY-SA 4.0

---

## What is K1SS

K1SS is a platform for building musical instruments from interchangeable modules.

The base unit connects to creative modules — sequencers, effect controllers, tactile surfaces, whatever the design calls for. Each configuration produces a different instrument. The platform is the constant; the instrument is the variable.

It is not a product line in the traditional sense. It is an open hardware platform with a growing module catalog, where the catalog is shaped by the people using it.

---

## M4Z3

M4Z3 is the first instrument built on the K1SS platform. It is a live performance controller for DJs and electronic performers.

The design premise: most DJ hardware is either made for the studio or made for demo units at a trade show. Neither is a live instrument. M4Z3 is built around what a performer actually needs on stage — not a marketing checklist.

### Native hardware for Mixxx

[Mixxx](https://mixxx.org) is free, open source DJ software. Approximately 2 million users. No hardware has ever been designed specifically for it — controllers exist with Mixxx mappings, but the hardware decisions were made independently of Mixxx's architecture.

M4Z3 is different. The hardware decisions start from the software. Physical controls are matched to how Mixxx models a performance, not retrofitted via MIDI mapping. The goal is a controller where the software and hardware have the same mental model.

---

## How the modular system works

A K1SS instrument has a central unit that handles audio, connectivity, and power. Modules connect to it and extend what the instrument can do. You configure the instrument by choosing which modules to attach.

Modules are interchangeable. If your setup changes, you change the modules. A module bought today is compatible with hardware released later — the connector specification is fixed and published.

There is no subscription, no cloud dependency, no feature that requires a server to exist in three years.

---

## Open source

Everything is public:

- Schematics and PCB layout files (KiCad)
- Enclosure source files
- Firmware source code
- Bill of materials
- Assembly documentation

You can build your own. You can modify it. You can manufacture it. CERN-OHL-S requires that derivatives remain open under the same terms — improvements to the design come back to the commons.

The firmware is GPL-3.0 for the same reason.

---

## Community design

The module catalog is not fixed by the manufacturer.

Registered community members vote on which module designs get manufactured next. Members can also submit new module concepts. There is no editorial filter — votes determine what gets prioritized, and a technical review follows before production commitment.

Voting records and proposals are tracked in this repository under [`/community`](community/).

---

## Right to repair

K1SS instruments are designed to be repaired by their owners:

- Full schematics are published — no black box
- Modules are physically replaceable, not integrated into a single board
- No proprietary connectors
- No firmware lock or authentication requirement
- Spare parts available separately

If a module fails five years from now, you can replace that module. You can diagnose it from the schematic. You can order the components yourself and fix it.

This is a design constraint, not a marketing claim. It affects every hardware decision made.

---

## Status

Pre-production. Hardware prototypes exist and are being refined. Firmware is in active development.

This repository contains design files and firmware as they develop. The architecture is stable; implementation details will change. Breaking changes will be documented.

Not everything is committed yet. Files will appear as they reach a state worth publishing.

For investors and partners, see the [`/investors`](investors/) directory.

---

## Repository structure

```
/hardware        KiCad source files, Gerbers, BOM, mechanical drawings
/firmware        Source code, build instructions, Mixxx mapping files
/docs            Assembly guides, module specs, connector spec
/community       Module proposals, vote results, design discussions
/investors      Project overview, product info, team — for prospective partners and investors
```

---

## Contributing

The project is early. Most useful contributions right now:

**Mixxx users and developers** — Feedback on the M4Z3 approach to mapping, problems with existing controller support in Mixxx, incorrect assumptions about how performers use DJ software.

**Hardware makers** — Design file review, build attempts, errata reports, anything that looks wrong.

**Module proposals** — Open an issue with the `module-proposal` label. Describe what the module does, why it isn't already covered, and what physical form it needs to take.

Pull requests for documentation and firmware are welcome. Hardware changes require a discussion before PR — manufacturing is constrained in ways that aren't obvious from the files alone.

See [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Who builds this

One person. Besançon, France.

---

## License

| Component     | License        |
|:--------------|:---------------|
| Hardware      | CERN-OHL-S 2.0 |
| Firmware      | GPL-3.0        |
| Documentation | CC-BY-SA 4.0   |

---

*K1SS — Get lost.*
