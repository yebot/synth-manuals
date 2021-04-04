# Robaux - 3PT

![Robaux - 3PT](./images/Robaux%20-%203PT/Robaux%20-%203PT.png)

## Tripot

In Tripot mode you can control three parameters of your Eurorack with just one knob - perfect for live performances.

You can set the voltage of the large knob individually for each channel. Whether from 0V to 5V, 5V to 0V or something in between. With the offset parameter you can determine whether the change is parallel to the big knob or whether it is moved to the beginning or the end.

You can use the CV input with an external CV source instead of the big knob.

| Element   | Description      |
| --------- | ---------------- |
| B C       | CV Amount        |
| 1 2 3     | Channel          |
| D E F     | Display CV Value |
| G H I     | Minimum 0V to 5V |
| J K L     | Offset -50 to 50 |
| M N O     | Maximum 0V to 5V |
| P Q R     | CV Output        |


## LFO

In LFO mode you can use the module as a triple modulation oscillator.

The big knob sets the main frequency. Each channel has an adjustable frequency multiplier.

You can seamlessly crossfade between sine, triangle, sawtooth and square and set the slew limit of each waveform.

You can use the CV input with an external CV source instead of the big knob.

Note that the output of the LFO is unipolar.

| Element   | Description      |
| --------- | ---------------- |
| B C | Main Frequency
| 1 2 3 | Channel
| D E F | Display CV Value
| G H I | Frequency Multiplier
| J K L | Waveform
| M N O | Slew limit
| P Q R | CV Output

## Chord Progression

In chord progression mode, you can output triads. Connect it to a CV keyboard and play harmonious chords.

You can select the root note between C to B and set the mode between major and minor. The seven matching chords are placed on the white keys of an octave. With the variation control you can spread the notes.

For each channel you can set whether the notes are quantized within an octave and also set a note offset to generate atonal chords.

| Element   | Description      |
| --------- | ---------------- |
| C | 1V/Oct
| G | Root Key C - B
| H | Major / Minor
| I | Variation
| 1 2 3 | Channel
| D E F | Display CV Value
| J K L | Note Compress
| M N O | Note Offset
| P Q R | CV Output

## Quantizer

In the quantizer mode you can use the module to quantize incoming notes on up to 25 different scales.

Connect a CV keyboard and you will always hit the perfect key! Each channel can use a different root key and scale. The individual scales are divided into five banks. In each bank there are five different scales.

You can use channel three **R** as gate output for channel one. Turn the trimmer **I** clockwise until it stops. If the quantized note is different from the previous one, a gate will be output.

| Element   | Description      |
| --------- | ---------------- |
| C | 1V/Oct
| 1 2 3 | Channel
| D E F | Display CV Value
| G H I | Root Key C - B
| J K L | Scale Bank 1 to 5
| M N O | Scale 1 to 5
| P Q R | CV Output

## Random Generator

You can use the module as a random generator. Plug in a trigger signal to generate three different random voltages.

You can set the minimum and maximum random voltage per channel. The voltages can be output linear, or as notes in the scales chromatic, major and minor.

| Element   | Description      |
| --------- | ---------------- |
| C | Trigger Input
| 1 2 3 | Channel
| D E F | Display CV Value
| G H I | Minimum Value
| J K L | Maximum Value
| M N O | Linear, Chr, Maj, Min
| P Q R | CV Output

## Sequencer

You can use the module as a step sequencer. Connect a clock source and let the sequencer play melodies with up to 8 steps. You can set the note values from trimmer 1 all the way clockwise to trimmer 4. The middle trimmer 5 defines the length of the sequence.

The sequencer outputs the linear voltage on channel one. The voltages are output chromatically on channels two and three. The sequence will be split if you reduce the number of steps and output separately on channel two and channel three.

| Element   | Description      |
| --------- | ---------------- |
| C | Clock Input
| D | Current Step
| E | Clock Display
| F | Current Note
| G H I | Step 1, 2, 3
| J K L | Step 8, 4
| M N O | Step 7, 6, 5
| P Q R | CV Output Lin, Chr

## Euclidean Rhythm

You can also use the module as an euclidean rhythm generator. Add a clock source to the CV input and the tripot will output trigger signals.

You can define per channel how long the sequence should be and how many pulses are sent in this time. With the rotation parameter you can move the sequence in time.

| Element   | Description      |
| --------- | ---------------- |
| C | Clock Input
| 1 2 3 | Channel
| D E F | Display Active Trigger
| G H I | Steps 1 to 16
| J K L | Pulses 1 to 16
| M N O | Offset
| P Q R | Trigger Output

## Calibration

To use the module correctly, it must be tuned or calibrated as accurately as possible. Press and hold the mode button **A** of the tripot when switching on your Eurorack system until a ring animation is displayed. You will then be in calibration mode. You can also enter the calibration mode by pressing the mode button for a few seconds.

Let the module warm up for a while. On the back of the module there is a trimmer for each CV channel to fine-tune the signal. Please note that these trimmers should be turned up completely before you start the calibration. Take a VCO and a tuner. If necessary, disconnect the oscillator from any plugged in cables.

Now connect the 1V/Oct of the oscillator to channel one **P** of the Tripot. In calibration mode, the 3PT sends a constant voltage on all three channels. Turn the big knob **B** of the Tripot counterclockwise as far as it will go to the left. Note that no cable is plugged into the CV input **C**.
**
**Connect the tuner to a neutral waveform output of the VCO and tune the oscillator to the note C1. Now turn the big knob **B** clockwise as far as it will go to the right.

Then turn trimmer **G** until your tuner shows the note C5. When you slowly turn the big knob counterclockwise again, your tuner should show the notes C4, C3, C2, and when the knob is turned all the way to the left, C1 again. Use the trimmers to correct the tuning as close as possible.

Repeat this step with channel two **G** and trimmer **H**, and with channel three **R** and trimmer **I**.

When all channels are tuned, press the Mode button and the Tripot is ready to operate.

[source](https://www.robaux.io/assets/files/3PTmanual.pdf)