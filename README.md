# A-Mini-Stereo-Digital-Audio-Processor-MSDAP-
The performance of the MSDAP is expected to be the same level as that of two general DSP chips for implementing two-channel FIR digital filtering in audio applications. 

The objective of this project is to implement a low-power mini_stereo digital audio processor, which includes two sperate channels located on the left and right side of human ears. It is programmed with a built-in finite input response filters with up to 256 coefficients. It is designed as a lower power and environmentally friendly electric device.

The MSDAP is a mini_stereo digital audio processor includes a finite input response filter which can operate the convolution operation, it is programmed inside implemented an efficient arithmetic unit based on single-bit shift-right and accumulate operations that can be derived from power of two (POT) coefficient representation. The FIR filter output can be expressed as: y(n)=2^(-1) (… 2^(-1) (2^(-1) (2^(-1)+u1)+u2)+⋯ )+u16 … (Eq1) uj=xj(1)+xj(1)+xj(2)+⋯+xj(rj),1≤j≤16… (Eq2) The rj is the total number of the POT (power of two) digits occurred among all filter POT coefficients. The input files are represented by x(k).

Features:

26.988MHz system clock
768kHz data clock (48kHz x 16bits)
16 bits input audio and 40 bits output audio
48kHz sampling frequency
256 coefficients per channel
Independent left& right channels with different coefficients
512 maximum operations per channel
Automatically sleeping mode when 800 all-zero input signals detected

The paper demonstrating the digital chip can be found on https://www.utdallas.edu/~zhoud/EE6306/MSDAP%20paper.pdf
