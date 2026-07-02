# YuSynth Panning Mixer/Output
An extensible version of the YuSynth Output mixer &amp; VC-panner, minus the tone control circuitry.
<img height=80% width=80% alt="image" src="https://github.com/user-attachments/assets/8300efa6-a854-46d0-918f-058112d55203" />

Very early in the construction of my modular synth it became obvious that I was going to need a multi-channel mixer as an output stage. I'd already built a few YuSynth modules, so his [Mixout-VC Panner](https://yusynth.net/Modular/EN/MIXOUT/index.html) seemed like a promising choice especially as I had an old dual VU meter which could be pressed into service.


The original design includes a passive tone control circuit (which I chose to omit) and uses a two-board architecture with the four VC panner circuits on one board and the mixer and output circuitry on another. My synth is in Eurorack format, so I wanted to keep the board sizes as small as possible (which also makes them cheaper!). I decided to use an alternative physical architecture with the mixer output board (board B in my design) as a motherboard, with two 2-channel VC-panner boards (board A) plugged into it using pin headers.

This allows easy extensibility by adding further 2-channel VC-panner boards mounted on their own panels, daisy-chained from a header on the motherboard. I have indeed added an additional pair of inputs since originally building the module. Details of the construction are shown in the [pictures](https://github.com/clarionut/YuSynth-Panning-Mixer-Output/tree/main/Pictures) folder. Note that the two VC-panner boards mounted on the motherboard have the header pins on the front side on one board and the back side on the other to keep the wiring as clean as possible. Most of the pin headers on the motherboard are on the back side of the board. The pictures also show the additional input board and panel.

I replaced the original non-backlit VU meter with one which can be illuminated, and soldered a 2 pin header to the back of the main power input connection with flying leads to the resistor/LED positioned behind the meter.

The [schematic](https://github.com/clarionut/YuSynth-Panning-Mixer-Output/tree/main/Schematic) folder contains PDFs of the schematic and layout for the VC-panner boards (A) and the motherboard (B). The Kicad projects for these are in their own individual subfolders.

I've also include the [gerbers](https://github.com/clarionut/YuSynth-Panning-Mixer-Output/tree/main/Gerbers) in case these are of direct use to anyone.
