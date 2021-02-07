# MRF101 HF AMP design

## Introduction
This repository contains multiple circuits board designs for a 100W HF Amp using a single MRF-101A transistor.   This design is based on a design by HF5L.   This design operates with a 48V Nominal supply at around 3.5 Amps of current.

Input match is good from 160M -> 6M band (1.8M -> 54 MHz).   Device has a between 16 -> 20 dB of gain depending on frequency.

## KICAD design files
The Main Amp Deck consists of the MRF101 transistor and input/output matching circuitry.
This can be found in the /Amp_Main_Deck/kicad folder in this repository.   The amplifier deck requires output filtering to remove odd harmonics produced by the Class AB amp.   The filters are selected per band of operation.

## Powering the Amp
The concept to power the amplifier design is to use 2 6S LiPo batteries in series.  This will provide a 44 -> 52v operating range.  Current plan is to use RC batteries and off the shelf chargers for portable operation.

## TODO
Design some BFP filters for each of the HF Amateur Radio bands, will need to develop a switch bank to select which filter should be in line.   Using BPF because this will provide some selectivity and limit the amount of bandwidth being sampled for a SDR receiver architecture.

