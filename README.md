# giaceccos-piano
Salamander Grand Piano V3 prepared as a patch for the Waldorf Quantum and Iridium synths.

## About giaceccos-piano n
This is an early, though successful attempt at bringing the [Salamander Grand Piano V3](https://archive.org/details/SalamanderGrandPianoV3) to my Waldorf Iridium Keyboard. The the preset should work nicely also on the Waldorf Quantum and the normal Iridium, but please let me know if it does not.

The original Salamander distribution of piano samples is made of a single sample every 3 semitones (C, D#, F#, A, C...) from A0 to C8, each recorded at 16 levels of velocity at 48kHz - 24 bit and at 44.1kHz - 16 bit. 

I have experimentally observed that I could only load in my Iridium's memory about 60 samples at 44.1kHz - 16 bit. Of the full Salamander range, I then decided to use only C3 to C5 included, and 3 velocities only per each note: 4, 9 and 14, corresponding to MIDI intervals 0-41, 42-84 and 85-127. This choice totals about 175Mb, that is more than I have available on my Iridium's "samples partition". I store the samples on an SD card that is left inserted in the Iridium. I presume that this will be necessary for most other users, unless you wipe your other patches' samples.

Note that you won't get an error message from the Iridium when you try load one sample too many in a Particle oscillator. The user interface will go back to the list of samples, and the sample you've just tried to load just won't be there. That is how I realized that I had topped the Iridium's memory.

## How to install
To learn how to import presets in the Quantum and Iridium, I suggest you watch Tim Shoebridge's video [here](https://youtu.be/2Oh6bUIs5TU), but with an exception to the conventional instructions. Because of the size of the samples, you shall not try import the samples _together_ with the `qpat` patch file. I suggest you rather do this:

1. Prepare a FAT-32 formatted SD card to store all samples - perhaps you have one already - and add the contents of the `for the SD card` folder.
2. Prepare a FAT-32 formatted USB drive, where you will save the preset _without the samples_, from the `for the USB drive` folder.
3. Insert the SD card in the Quantum / Iridium SD card slot
4. Import the preset from the USB drive.

## License
Salamander Grand Piano V3 - that is partly re-distributed with this - is licensed for reuse under the Creative Commons Attribution 3.0 license. My additional work is licensed for reuse under the Creative Commons Attribution 4.0 International license.
