# DoublePlusBass
Full featured kick drum inspired by Thomas Henry's Bass+

Thomas Henry's Bass+ kick drum (wood block, tom) circuit is a masterclass in maximum functionality from a minimal part count. He got an extremely competent, versatile drum circuit out of one LM13700, a dual op amp, and passive components. I remain shocked and amazed by his ingenuity and elegant circuit design.

However, the Bass+ has some shortcomings, which I won't go into, instead, I'll just say that after building a Bass+ and playing it at a venue with a gigantic subwoofer, I felt driven to develop the concept farther, so here's my DoublePlusBass.

At the core of this module is a triangle(ish) wave VCO from the LM13700 datasheet. The base pitch of the VCO can be controlled with CV, with a trimmer to be able to get the response to the 1V/octave standard. The waveshape can be adjusted from the sligthly spiked triangle, through a sine wave, to a folded square wave. Buzzy to clean to *filthy*. The decay can be wood-block short, up to absurdly long, especially if you choose to build your copy with a larger capacitor.

The second row of potentiometers offer the ability to select how high the pitch sweep will rise. At the maximum setting, you can get crazy disco-tom sounds. The second potentiometer selects the pitch sweep decay, from a very punchy short sweep to a gradual decay. The third knob allows you to select the style of pitch sweep: the 909-style is the disco-tom or punchy kind of pitch sweep that decays more quickly at the beginning. The 808 kick drum circuit uses a totally different way to get the oscillation, so the pitch sweep is much more stable during the body of the kick sound, sagging off more near the end of the sound. The pitch of the drum will be much higher as you turn the knob toward the 808-style position, so you'll need to adjust the master pitch knob lower to get a classic deep 808 sound out of your DoublePlusBass.

The third row of potentiometers controls the impact sound, whether it's a sharp treble-heavy spike or a low DC voltage THUMP, and then how loud that transient sound will be. Between these two pots are a pair of LEDs. These LEDs light up when the kick drum is active, and their brightness represents the amount the voltage coming out of the "ENVELOPE" jack is lowered. The "ENVELOPE" voltage can be used to "turn down" some other signal or group of signals with a VCA.

The fourth and final row of potentiometers: the left potentiometer attenuates the CV that controls the pitch of the drum. The second potemtiometer controls the amount the envelope sags when the kick drum is active. The last potentimeter is a volume control.

The row of jacks: the first is the trigger in. This can be anything from 3V to full rail voltage, and I haven't found a trigger that won't work. Even a silly audio-rate triangle wave will trigger the drum. The second is the CV in. The third is the envelope out, use that voltage to duck other signals. The last jack is the output.

The PCB has text on it to customize your own build with some through-hole parts, specifically a resistor which limits how high the pitch can go, a film capacitor which can set the range of how low the pitch can go, and one of the electrolytic capacitors will set the maximum length of the decay. It may be tempting to just max out all of these parameters (tempting to me, at least) but remember that if, for example, you've chosen a REALLY LONG MAXIMUM DECAY TIME, it will be harder to dial in a short punchy kick drum sound at the minimum setting of that dial.
