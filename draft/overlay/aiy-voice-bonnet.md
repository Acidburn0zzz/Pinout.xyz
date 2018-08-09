<!--
---
name: AIY Voice Bonnet
class: board
type: audio,sensor
formfactor: pHAT
manufacturer: Google
description: A pHAT that helps you build an intelligent speaker with voice recognition that connects to the Google Assistant
url: https://aiyprojects.withgoogle.com/voice
github: https://github.com/google/aiyprojects-raspbian
image: 'aiy-voice-bonnet.png'
pincount: 40
eeprom: yes
power:
  '1':
  '2':
ground:
  '6':
  '9':
  '14':
  '20':
  '25':
  '30':
  '34':
  '39':
pin:
  '3':
    mode: i2c
  '5':
    mode: i2c
  '8':
    mode: uart
    name: TXD breakout
  '10':
    mode: uart
    name: RXD breakout
  '12':
    mode: i2s
    name: I2S BCLK
  '16':
    mode: gpio
    name: Button
  '33':
    mode: i2s
    name: I2S LRCLK
  '38':
    mode: i2s
    name: I2S SDIN
  '40':
    mode: i2s
    name: I2S SDOUT
-->
# AIY Voice Bonnet

The AIY Voice Bonnet comes with the AIY Voice Kit (V2) by Google—a do-it-yourself intelligent speaker. The Voice Bonnet connects to a Raspberry Pi Zero to create a natural language processor that can connect to the Google Assistant.

The bonnet includes on-board hardware to facilitate audio capture and playback, stereo speaker terminals, a headphone jack, an 8-pin button connector, UART breakout pins, and 4 unique GPIO pins called `PIN_A`, `PIN_B`, `PIN_C`, and `PIN_D`.

If you have the V1 Voice Kit (full size HAT for Raspberry Pi 3), instead see the [Voice Hat](/pinout/aiy_voice_hat).
