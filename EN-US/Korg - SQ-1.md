# Korg - SQ-1 <!-- omit in toc -->

- [SEQUENCER MODE Selector (left to right)](#sequencer-mode-selector-left-to-right)
- [(power) button](#power-button)
  - [Auto power-off function](#auto-power-off-function)
- [littleBits OUT jack](#littlebits-out-jack)
- [OUT (MIDI OUT) jack](#out-midi-out-jack)
- [CV - A OUT - GATE, CV - B OUT - GATE jacks](#cv---a-out---gate-cv---b-out---gate-jacks)
- [IN - SYNC - OUT jacks](#in---sync---out-jacks)
- [(USB) jack](#usb-jack)
- [SPEED knob](#speed-knob)
- [DUTY knob](#duty-knob)
- [PLAY/STOP button](#playstop-button)
- [FUNCTION button](#function-button)
  - [CV A RANGE, CV B RANGE](#cv-a-range-cv-b-range)
  - [CV A BEHAVIOR, CV B BEHAVIOR](#cv-a-behavior-cv-b-behavior)
- [Step knobs](#step-knobs)
- [Step buttons](#step-buttons)
- [MODE/CLEAR button](#modeclear-button)
  - [GATE ON/OFF](#gate-onoff)
  - [ACTIVE STEP](#active-step)
  - [SLIDE](#slide)
  - [STEP JUMP](#step-jump)
- [Global parameter settings](#global-parameter-settings)
  - [Auto power-off function](#auto-power-off-function-1)
  - [MIDI channel setting](#midi-channel-setting)
  - [GATE output polarity of channel A and channel B](#gate-output-polarity-of-channel-a-and-channel-b)
  - [SYNC IN and SYNC OUT polarity](#sync-in-and-sync-out-polarity)
  - [Sequence step resolution](#sequence-step-resolution)
- [About the MIDI implementation chart](#about-the-midi-implementation-chart)

## SEQUENCER MODE Selector (left to right)

Specifies the sequencer mode

1. Channel A and channel B run alternately in units of one step; signals are output from the CV-A OUT-GATE and CV-B OUT-GATE jacks. Use channel A and channel B to control pitch or other parameters.
2. The steps run in the order of channel A → channel B; signals are output from the CV-A OUT-GATE and CV-B OUT-GATE jacks. Use channel A and channel B to control pitch or other parameters.
3. Channel A and channel B run in parallel, and reverse direction at the last step. Use channel A and channel B to control pitch or other parameters. Channel A signals are output from the CV-A OUT-GATE jacks, and channel B signals are output from the CV-B OUT-GATE jacks.
4. Channel A and channel B run in parallel. Use channel A and channel B to control pitch or other parameters. Channel A signals are output from the CV-A OUT-GATE jacks, and channel B signals are output from the CV-B OUT-GATE jacks.
5. **CV DUTY** - Only channel A runs; signals are output from the CV-A OUT-GATE and CV-B OUT-GATE jacks. Use channel A to control pitch or other parameters. Use channel B to control the duty cycle of the gate signal.
6. **CV SLIDE** - Only channel A runs; signals are output from the CV-A OUT-GATE and CV-B OUT-GATE jacks. Use channel A to control pitch or other parameters. Channel B controls how smoothly the values for each step of channel A are connected.
7. **CV DUTY RANDOM** - The steps of channel A run randomly; signals are output from the CV-A OUT-GATE and CV-B OUT-GATE jacks. Use channel A to control pitch or other parameters. Use channel B to control the duty cycle of the gate signal.
8. **RANDOM** - The steps of channel A and channel B run randomly; signals are output from the CV-A OUT-GATE and CV-B OUTGATE jacks. Use channel A and channel B to control pitch or other parameters.

## (power) button

This button turns the power on. To turn the power off, press and hold the
button for approximately one second.

### Auto power-off function

The SQ-1 has an auto power-off function. When approximately four hours have elapsed without the SQ-1 running, the power will turn off automatically. You can disable the auto power-off function (see ”Global parameter settings”)

## littleBits OUT jack

Connect this jack to a littleBits unit that you want to control.

## OUT (MIDI OUT) jack

Use the included adapter cable and a MIDI cable to connect this jack to an external MIDI unit that you want to control.

## CV - A OUT - GATE, CV - B OUT - GATE jacks

Connect these jacks to an external analog unit that you want to control. The CV jacks output signals that control pitch or other parameters, and the GATE jacks output gate signals that control the length of the notes.

## IN - SYNC - OUT jacks

Connect these jacks to an analog synthesizer such as the volca series or the monotribe, so that the two units will operate in synchronization. The SYNC OUT jack outputs a 5V pulse that’s 15 ms long at the beginning of each step. If you connect the SYNC OUT jack of a volca series unit or the monotribe to the SYNC IN jack of the SQ-1, the step clock of the SQ-1 is ignored, and steps advance according to the pulses that are input. Use this if you want steps to synchronize to the pulses that are output from a monotribe or other analog sequencer, or from an audio output of your DAW.

## (USB) jack

Connect this to your computer if you want to control a software synthesizer from the SQ-1. The USB connection is also used to update the SQ-1’s operating system software. If this is connected, the SQ-1 will be powered by USB bus power.

## SPEED knob

Controls the speed at which the sequencer runs

## DUTY knob

Adjusts the duty cycle of the gate signal. Higher values make the notes sound longer.

If the sequencer mode is or , the setting of this knob is ignored, and the duty cycle is controlled by channel B.

## PLAY/STOP button

Starts/stops the sequencer

## FUNCTION button

By holding down this button and pressing the STEP buttons of each channel, you can edit the CV output parameters of each channel. The button is lit up while you are editing these settings.

### CV A RANGE, CV B RANGE

These parameters specify the voltage of the channel A or channel B CV output jacks. Set this to either 1V, 2V, 5V, or 8V [Hz/V] as appropriate for the device that’s connected. Note: The voltage setting affects the range of pitches that are sounded. For the appropriate voltage setting, refer to the manual of the connected device.

### CV A BEHAVIOR, CV B BEHAVIOR

These parameters specify how the setting of each step’s knob will affect the output when using channel A or channel B to control the pitch.

- **LINEAR**: The setting of each step’s knob is output without any adjustment.
- **MINOR**: The setting of each step’s knob is adjusted to a minor scale for output.
- **MAJOR**: The setting of each step’s knob is adjusted to a major scale for output.
- **CHROMA**: The setting of each step’s knob is adjusted to a chromatic scale for output.

## Step knobs
These specify the value for each step of channel A and channel B.

## Step buttons

These edit the parameter that’s specified by the MODE button.

## MODE/CLEAR button

This button lets you edit the parameters of channel A and channel B. The editable parameter changes each time you press a button. Use the step buttons of each channel to edit the setting.

The settings are reset if you hold down the FUNCTION button and press the MODE button (GATE ON/OFF: all steps on, ACTIVE STEP: all steps on, SLIDE: all steps off).

### GATE ON/OFF

This function specifies whether each step’s gate output is on or off. Steps that are off (button unlit) do not output a signal from the CV/GATE jacks during playback.

### ACTIVE STEP

This feature specifies whether each step of the sequence is on or off. Steps that are off (button unlit) are disabled, and are excluded from the sequence.

### SLIDE

This feature allows you to specify how the value changes between steps. If this is on (button lit up), the pitch or value changes smoothly from one step to the next. If the sequencer mode is , the settings of each step of channel B will be used.

### STEP JUMP

If the sequencer is running, pressing a step button will cause the sequencer jump immediately to that step. If the sequencer is stopped, pressing a step button (the button lit up) makes the sequencer start running from that step.

## Global parameter settings

If you turn on the power while pressing the PLAY/STOP button, you can set the following global parameters. When you’ve finished editing the settings, press the button. The settings will be saved and the SQ-1 will restart.

### Auto power-off function

To enable the auto power-off function, make the PLAY/STOP button light up. With the original factory settings, this feature is enabled. To disable the auto power-off function, make the PLAY/STOP button unlit.

### MIDI channel setting

The channel A and channel B step buttons correspond to MIDI channels 1‒16. Press the button of the corresponding channel to make it light up.

### GATE output polarity of channel A and channel B

When the MODE button lit is lit up + (positive polarity) is selected. When the MODE button is unlit (negative polarity) - polarity is selected. With the factory settings enabled, + (positive polarity) is selected. Set this as appropriate for the device that’s connected.

### SYNC IN and SYNC OUT polarity

When the MODE button is lit + polarity (rise) is selected. When the MODE button is unlit - polarity (fall) is selected. With the factory settings enabled, + (rise) is selected. Set this as appropriate for the device that’s connected.

### Sequence step resolution

Use the SEQUENCER MODE selector to specify the resolution of the steps.

- First position = quarter notes
- Second position = eighth notes
- Third position = sixteenth notes

## About the MIDI implementation chart

You can connect the SQ-1’s MIDI OUT connector to an external MIDI device and control it. The MIDI messages that the SQ-1 can transmit are listed in the MIDI implementation chart. You can download the SQ-1’s MIDI implementation chart from the [Korg website](http://www.korg.com).

[source](https://www.korg.com/us/support/download/manual/0/436/2017/)