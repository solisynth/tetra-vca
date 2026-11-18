# TETRA VCA #

### Quad Linear/Exponential VCA and Mixer ###

<!-- TODO: add a photo, e.g. pictures/tetra-vca_front.jpg
<p align="center">
  <img src="pictures/tetra-vca_front.jpg" alt="TETRA VCA front panel" width="50%">
</p>
-->

TETRA VCA has four voltage-controlled amplifiers in 12 HP, built around the SSM2164 quad VCA chip. Each channel has a level knob, a CV input with its own amount control, and a switch to choose between a linear and an exponential response, so it works just as well for shaping envelopes on audio as for processing CV.

The CV inputs are normalled from one channel to the next: a single CV patched into channel A also controls B, C and D until you patch something else further down. The outputs are normalled too: unpatched outputs are summed into the next channel, so the module also works as a four-channel mixer with the last output carrying the mix.
A bicolour LED per channel shows the level <!-- TODO: what does red/green mean? -->.
<!-- TODO: verify the normalling description (CV A→B→C→D, OUT A→B→C→D) against the actual behaviour -->

## Get one
TETRA VCA is available from [Solisynth](https://solisynth.com/). <!-- TODO: link the product page and say what the kit includes -->

## Features
- 4 VCAs based on the SSM2164
- Linear / exponential response switch per channel
- Level (offset) knob per channel
- CV input with amount control per channel <!-- TODO: attenuator or attenuverter? panel shows "-|+" and "o|+" -->
- CV inputs normalled A → B → C → D
- Outputs normalled into the next channel: unpatched channels mix into the following output
- Bicolour LED per channel
- DC-coupled <!-- TODO: confirm -->

## Specifications
| | |
|---|---|
| Width | 12 HP |
| Depth | <!-- TODO --> mm |
| Power +12 V | <!-- TODO --> mA |
| Power −12 V | <!-- TODO --> mA |

## Hardware
The schematics and PCB layouts are KiCad projects:

- `tetra-vca-main-pcb/`: main PCB and jack/control board (schematic split into one sheet per channel plus the power supply)
- `tetra-vca-frontpanel-pcb/`: front panel

<!-- TODO: add a BOM (csv and/or ibom.html) like the other modules -->
Gerbers and BOMs can be generated from the KiCad projects.

## Repository structure
| Folder | Contents |
|---|---|
| `tetra-vca-main-pcb/` | KiCad project for the PCBs |
| `tetra-vca-frontpanel-pcb/` | KiCad project for the front panel |
| `pictures/` | Photos of the module |

## License
TETRA VCA is open source:

- Hardware: [CERN-OHL-S-2.0](LICENSES/CERN-OHL-S-2.0.txt)
- Documentation: [CC-BY-SA-4.0](LICENSES/CC-BY-SA-4.0.txt)

If you share a modified version or hardware built from these files, it has to stay open source under the same license.
"Solisynth", "TETRA VCA" and the Solisynth logo are not covered by these licenses: derivatives must use their own name and branding. See [LICENSE.md](LICENSE.md) for details.
