
# QPSK Baseband Transceiver: AWGN and BER Analysis

## Overview

This project focuses on the design and simulation of a Quadrature Phase Shift Keying (QPSK) baseband communication system over an Additive White Gaussian Noise (AWGN) channel.

The primary objective is to understand the performance of a digital communication system by analysing the relationship between Signal-to-Noise Ratio (SNR) and Bit Error Rate (BER).

The project implements the fundamental stages of a digital communication transceiver, including bit generation, QPSK modulation, AWGN channel modelling, demodulation, and BER calculation.

## Objectives

- Design a QPSK baseband transmitter and receiver.
- Understand the principles of digital phase modulation.
- Simulate signal transmission through an AWGN channel.
- Investigate the impact of noise on communication reliability.
- Calculate BER at different SNR levels.
- Analyse the simulated BER performance against theoretical expectations.

## System Architecture

The communication system consists of the following functional blocks:

```text
     Random Bit Generation
              |
              v
        QPSK Modulator
              |
              v
       AWGN Channel
              |
              v
        QPSK Demodulator
              |
              v
      Recovered Bit Stream
              |
              v
         BER Analysis
```

## Theoretical Background

### 1. Quadrature Phase Shift Keying (QPSK)

QPSK is a digital modulation technique that transmits two bits per symbol by representing information through four distinct carrier phase states.

Each symbol represents one of four possible phase values, allowing QPSK to transmit twice as many bits per symbol as Binary Phase Shift Keying (BPSK).

### 2. Additive White Gaussian Noise (AWGN)

An AWGN channel is a mathematical model used to represent the effect of random noise on a transmitted signal.

The received signal can be represented as:

r(t) = s(t) + n(t)

Where:

- r(t) = Received signal
- s(t) = Transmitted signal
- n(t) = Additive White Gaussian Noise

### 3. Bit Error Rate (BER)

BER measures the proportion of incorrectly received bits compared to the total number of transmitted bits.

BER = Number of Incorrectly Received Bits / Total Transmitted Bits

A lower BER indicates better communication system performance.

### 4. Signal-to-Noise Ratio (SNR)

SNR represents the ratio of signal power to noise power.

An increase in SNR generally results in reduced noise interference and improved BER performance.

## Simulation Methodology

The simulation follows these main stages:

1. Generate a random binary data sequence.
2. Group binary data into pairs for QPSK symbol mapping.
3. Modulate the binary data using QPSK.
4. Transmit the modulated signal through an AWGN channel.
5. Demodulate the received signal.
6. Compare transmitted and received binary sequences.
7. Calculate BER for different SNR values.
8. Analyse the BER performance.

## Performance Analysis

The performance of the QPSK transceiver is evaluated by observing BER variations across different SNR levels.

The simulated results can be compared with theoretical QPSK performance to assess the accuracy of the implementation.

For coherent QPSK over an AWGN channel with Gray coding, the theoretical BER is:

Pb = Q(sqrt(2Eb/N0))

Where:

- Pb = Probability of bit error
- Eb = Energy per bit
- N0 = Noise power spectral density
- Q(.) = Gaussian Q-function

## Technologies and Tools

- MATLAB
- Digital Signal Processing
- Digital Communication Systems
- QPSK Modulation and Demodulation
- AWGN Channel Modelling
- BER and SNR Analysis

## Repository Structure

```text
QPSK-Baseband-Transceiver-AWGN-BER-Analysis/
│
├── README.md
│
├── MATLAB/
│   └── [Simulation Files]
│
├── Results/
│   └── [BER Performance Plots]
│
└── Documentation/
    └── [Project Documentation]
```

## Applications

QPSK modulation is widely used in:

- Satellite communication systems
- Wireless communication networks
- Digital radio communication
- Space communication systems
- Modern digital transmission systems

## Conclusion

This project demonstrates the fundamental operation and performance evaluation of a QPSK baseband communication system under AWGN channel conditions.

By analysing BER against SNR, the project provides insight into the relationship between channel noise and digital communication reliability.

## Author

**Gul Afroz Ifra Khan**

BS Avionics Engineering  
Institute of Space Technology (IST)

GitHub: https://github.com/GulAfrozIfra

---

*This repository is intended for educational, academic, and engineering research purposes.*
