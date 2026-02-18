<details>
<summary>Experiment 11 - Sampling and reconstruction</summary>

### Objectives
- To be familiar with digital transmission
- To understand the principles of PAM and Quantization

### Introduction
A digital transmission is a process of conveying information into  a discrete-time signal by measuring its amplitude at regular intervals. process called sampling takes measurements of the continuous message signal time intervals into a discrete-time signal. in this experiment, we will demonstrate the 2 common sampling techniques: natural sampling and sample-and-hold sampling.

A natural sampling is a form of modulation technique that involves multiplying the analog signal to the pulse train(rectangular pulses), this will allow to follow the orignal waveform's shape during pulse duration, if the pulse is on, input signal passes through, if the pulse if off, no signal will output. A sample-and-hold(S&H) is an electronic device that takes the message's amplitude signal in each point and holds the value constant for a duration.

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2011/Sampling%20demo.JPG" />
</div>

### Block diagram: Natural sampling

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2011/Natural%20sampling%20BD.JPG" />
</div>

baed on the diagram, it shows that the 2kHz signal will be our information signal, connected to the input of the dual analog switch, the 8kHz digital signal will serve as the switching component or the sampling frequency that will let the input signal pass to the output whenever the control signal is in positive peak and blocks it when the control signal is in 0V, generating a Pulse amplitude modulation(Natural sampling).

### Setup: Natural sampling

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2011/Natural%20sampling%20setup.jpg" />
</div>

### Output

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Natural%20sampling%20output.jpg" />
</div>

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Natural%20samping%20and%20message%20comparison.jpg" />
</div>

as expected, the signal will get pass through when the sampling frequency is at positive peak voltage, and blocks it when it reach the negative peak voltage, forming a Natural sampling.

### Block diagram: Sample and hold/w tunable LPF(message reconstruction)

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2011/S%26H%20%20and%20reconstruction%20BD.jpg" />
</div>

Based on the block diagram, the dual analog switch circuit will be replaced with Sample-and-hold circuit, the princple of S&H sampling is that it holds the first constant value until the next sampling frequency 

### Setup: Sample and hold sampling/w tunable LPF(message reconstruction)

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2011/Sample%20and%20hold%20%20original%20message%20reconstruction%20setup.jpg" />
</div>

### Output: Sample and hold sampling/w tunable LPF(message reconstruction)

- S&H Output
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Sample%20and%20hold%20output.jpg" />
</div>

- Original message and S&H comparison

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/S%26H%20and%20message%20comparison.jpg" />
</div>

- Reconstructed Message to Original message comaparison

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/S%26H%20Reconstructed%20message%20comparison.jpg" />
</div>

### Observation

if the sampling frequency increased, it improved the quality of the reconstruction of the signal because it reduces aliasing and provides improves the quality when it comes to reconstructing the signal

### Setup: Natural sampling using VCO

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2011/Observation%20setup/Natural%20sampling%20setup.JPG" />
</div>

### Output: Natural sampling using VCO

- if VCO frequency is low

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Observation%20output/Natural%20sampling%20under%20low%20frequency%20sampling.JPG" />
</div>

- if VCO frequency is high

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Observation%20output/Natural%20sampling%20under%20high%20frequency%20sampling.JPG" />
</div>

### Setup: S&H Sampling using VCO

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2011/Observation%20setup/S%26H%20Sampling%20VCO%20observation%20setup.JPG" />
</div>

### Output: S&H Sampling using VCO

- if VCO frequency is low
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Observation%20output/S%26H%20under%20low%20frequency%20sampling.JPG" />
</div>

- if VCO frequency is high
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2011/Observation%20output/S%26H%20under%20high%20frequency%20sampling.JPG" />
</div>

</details>

<details>
<summary>Experiment 12 - PCM encoding</summary>

### Objectives
- To familarize PCM Encoding
- Understand the basic principle of Pulse Code Modulation (PCM)
- Analyze the PCM output for 0V input and variable DC input.
- Compare and observe the relationship between the analog input voltage and the generated PCM digital data.
### Introduction

A pulse code modulation(PCM) is a type of digital modulation technique that converts analog signal into binary sequence of 1s and 0s. PCM uses sampling, quantizing, and encoding in order for analog signal to be converted into binary system. This process was developed in 1937, primarily used for telephony, space communications, and digital audio processing during the 1960s and 70s.

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2012/PCM%20demo.JPG" />
</div>

<div align="center">
<img width="800" height="800" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2012/PAM%20Steps.JPG" />
</div>

<div align="center">
<img width="800" height="800" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2012/block%20of%20encoding%20PCM.jpg" />
</div>

PCM contains 2 output pins:
- Frame synchronization - it is an identifier that will align to the exact beginning of the data frame of an encoded data to identify and read the PCM data from the moment the bit starts and stops.
- PCM data - this is the equivalent analog signal convered into digital data that has been decoded, in our setup, the EMONA telecoms trainer only has a 7 bit encoder.

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2012/PCM%20Data%20actial%20representation.jpg" />
</div>
  
### Block diagram

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2012/PCM%20Encoder%20with%200V%20Input.JPG" />
</div>

our input signal will be grounded and our clock signal would be 8kHz signal. the PCM encoder for EMONA combines the process of Sampling, Quantization, and encoding into a single block, making it easy to implement rather than using a separate dual analog switch for sampling and quantization.

### Setup

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2012/FS%20and%20Digital%20signal%20comparison.jpg" />
</div>

Observing the output, the frame synchronization (FS) signal appeared as a periodic pulse that marked the beginning of each data frame. The 8 kHz clock signal was visible and maintained a constant frequency, which means it has a stable sampling operation

### Output

- CH1(Frame synchronization) and CH2(8kHz digital clock signal) comparison
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2012/Clock%20signal%20and%20Frame%20synchonization%20signal.jpg" />
</div>

- CH1(Frame synchronization) and CH2(PCM DATA) comparison
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2012/Frame%20synchronization%20and%20PCM%20output%20data.jpg" />
</div>

- Reading the equivalent binary data of the PCM output

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2012/PCM%20Data%20reading.JPG" />
</div>

### Block diagram

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2012/PCM%20Encoder%20with%20Variable%20DC%20Input.JPG" />
</div>

### Setup

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2012/PCM%20Setup%20DCV.jpg" />
</div>

Modifying the setup, this time, instead of grounded input, we use the variable dc voltage and observe the output.

### Output

https://github.com/user-attachments/assets/9bb37632-e221-4fab-a63e-4295a544365a


The binary code pattern shifted based on the amplitude of the applied DC voltage. Higher DC voltages produces more binary codes corresponding to higher quantization levels, while lower DC voltages produced less binary codes.

### Additional observation

Looking at the converted binary data of the PCM output at 0V, it shows that the data is not 000000 when the input is 0V. This is because most PCM coding uses a bipolar encoding scheme, where the mapping range usually from -2V to +2V across 256 steps. which means 0V is around the middle point, resulting to a minimum binary value rather than a complete 00000000 binary output, another reason is the Quantization levels where 0V may not align exactly wih the first quantization level due to the ADC dividing the total voltage span. Also, when looking at the second output where we applied a variable DC voltage, the output keeps changing even when the value of the input voltage is constant, this is probably because  the voltage is different for every sample input signal, or possibly due to small noise variation.


</details>

<details>
<summary>Experiment 13 - PCM decoding</summary>


### Objectives

- To familiarize with the operation of the PCM Decoder module in the EMONA Telecommunications Trainer.
- Understand the basic principle of PCM decoding and signal reconstruction.
- To create a PCM decoder.
- Analyze and compare the reconstructed output signal with the original input signal.

### Introduction

Pulse Code Modulation (PCM) decoder is the counterpart of the PCM encoder used to convert encoded PCM data back into its original analog signal. the decoder performs the process to reconstructing the signal, it receives the PCM data along with the clock frequency and the frame synchronization signals to ensure correct timing and proper alignment of each digital word. for our experiment, we'll stole the clock frequency and the frame synchronization to the encoder to make sure that the orignal message is recovered

### Block diagram

- Before filtering
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2013/PCM%20Encoder%20and%20Decoder%20BD.JPG" />
</div>

- After filtering

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2013/PCM%20Encoder%20and%20Decoder%20before%20filtering%20BD.JPG" />
</div>


### Setup

- Before filtering
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2013/PCM%20Decoder%20setup.jpg" />
</div>

- After filtering

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2013/PCM%20decoder%20setup%20with%20tunable%20LPF.jpg" />
</div>

### Output

- Before filtering

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2013/PCM%20decoder%20output.jpg" />
</div>

- After filtering

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2013/PCM%20decoder%20output%20after%20filtering.jpg" />
</div>

### Additional Observation

Looking at the signal before the output uses LPF, the decoded output appears to be a steps, similar to a sample-to-hold sampling. This is because PCM decoders uses Digital to analog converter, which generally converts the PCM data to an equivalent analog signal based on the information the PCM data contains. Looking back at the encoding side, the Emona Telecoms trainer combines the 2 stages of generating a PAM before the input signal to be encoded: Sampling and Quantization. The signal must be converted into a discrete signal(equivalent to steps of analog signal) before it is encoded into a Pulse code.

<div align="center">
<img width="800" height="800" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2012/PAM%20Steps.JPG" />
</div>

when decoding the PCM data, it shows the exact output we should expect, which is the quantized data. using tunable LPF will smooth out the decoded PCM data and turn it into its orignal waveform.

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2013/Block%20of%20decoding%20PCM.jpg" />
</div>

</details>


<details>
<summary>Experiment 14 - BW limiting and restoring digital signals</summary>

### Objectives

- To famlliarize bandwidth limiting
- understand its effects in digital transmission
- observe its effects in different digital modulation techniques
- Analyze dthe istortion caused by a low-pass filter.
- Restore a distorted digital signal using a comparator



### Introduction

A medium acts as a filter, it lets a range of singal frequency pass unaffected while outside the frequency range are attenuated, if the bandwidth is not wide enough, the original message can cause distortion or partially loss of information, one of the most usefulBandwidth limiting is a process of limiting the frequency range of a signal, reducing the high-frequency components of the signal that cause rounding of sharp edges when recovering the message. Bandwidth limiting has an advantage when it comes to improving signal recovery,  blocking unwanted high-frequency signals that causes attenuation/distortion to the recovered information.

### Block diagram - PCM decoding with bandwidth limiter
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2014/Bandwidth%20limiting%20on%20PCM%20decoding.jpg" />
</div>


### Setup - PCM decoding with bandwidth limiter

- Without LPF(Bandwidth limiter)
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2014/Digital%20signal%20modeling%20with%20bandwidth%20limiter%20setup.jpg" />
</div>

- With LPF(Bandwidth limiter)

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2014/Digital%20signal%20modeling%20with%20bandwidth%20limiter%20and%20%20signal%20restoration%20setup.jpg" />
</div>

Based on the block diagram, we'll construct a PCM decoder with and without the bandwidth limiter and compare its effects after adding the LPF across the channel. 

### Output- PCM decoding with bandwidth limiter

- Without LPF(Bandwidth limiter)
  
https://github.com/user-attachments/assets/475d4c45-1348-4017-8844-98d8da1195f0

- With LPF(Bandwidth limiter)

  https://github.com/user-attachments/assets/387ec482-36ee-42d2-afc5-15907743c411

comparing both output, when looking at the signal without the bandwidth limiter, the output of the decoded signal moves smooth when we vary the VDC signal, meanwhile adding the LPF(bandwidth limiter) across the channel looks distorted when we vary the VDC and returns into its normal output

### Block diagram - Digital modeling with bandwidth limiter

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2014/Sequence%20generator%20with%20SYNC%20to%20EXT.JPG" />
</div>

- Signal recovery

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2014/Bandiwdth%20limiting%20on%20sequence%20generator.JPG" />
</div>


### Setup - Digital modeling with bandwidth limiter

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2014/Digital%20signal%20modeling%20with%20bandwidth%20limiter%20setup.jpg" />
</div>

- Signal recovery

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment 14/Digital signal modeling with bandwidth limiter and%20 signal restoration setup.jpg" />
</div>

### Output - Digital modeling with bandwidth limiter

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2014/digital%20signal%20modeling%20with%20bandwidth%20limited%20digital%20signal%20output.jpg" />
</div>

- Signal recovery

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2014/digital%20signal%20modeling%20recovery%20otuput.jpg" />
</div>

</details>

<details>
<summary> Experiment 15 - Amplitude Shift Keying(ASK) </summary>

### Objectives
- To be familiarize with Amplitude Shift Keying
- understand the basic principle of Amplitude Shift Keying.
- Implement Amplitude Shift Keying
- restore the digital signal into its orignal form
- observe its output

### Introduction

A Amplitude Shift Keying (ASK) is a type of digital modulation technique in which the amplitude of a carrier signal is varied according to the digital data, while the frequency and phase remain constant. In simple terms, ASK uses different amplitude levels to represent binary data (1s and 0s).

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2015/ASK%20demo.JPG" />
</div>

### Block diagram

- ASK Generator
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2015/ASK%20Generator%20BD.JPG" />
</div>

for Amplitude Shift Keying generation, we'll need  a Dual analog switch, the Master signal will serve as the input for the analog switch, and  the sequence generatr will serve as the digtal data. the ASK will be generated based on the switching of the sequence generator, where the master signals acts as the carrier. if the voltage of the sequence generator switch to positive(1), the master signal will flow to the output signal of the dual analog switch, and if the digital signal siwtch to negative(0), no signal will be not flow to the output of the analog switch, generating the ASK signal. 

- Envelope detector(Demodulator)

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2015/ASK%20Envelope%20detector%20BD.JPG" />
</div>

for this setup, we'll deodulate the signal using an envelope detector, it has the same setuo with AM demodulation, but for digital modulation. the input is modified with a 100kHz master signal. It does this by extracting the envelope of the amplitude-modulated signal which  corresponds to the digital "1"s and "0"s.

- Digital data reconstruction

 for this setup, this will reconstruct the generated ASK signal into its orignal data, it uses a comparator to convert the analog envelope into clean digital pulses. The comparator compares the voltage signal of the envelope detector, reconstructing the original digital data.
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2015/ASK%20Digital%20signal%20recovery%20BD.JPG" />
</div>

### Setup

- Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2015/ASK%20Generation%20setup.jpg" />
</div>
  
- Envelope detector

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2015/ASK%20Envelope%20detector%20setup.jpg" />
</div>

- Digital data reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2015/ASK%20digital%20signal%20recovery%20setup.jpg" />
</div>
  
### Output

- Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2015/ASK%20Output.jpg" />
</div>
  
- Envelope detector

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2015/ASK%20Output.jpg" />
</div>

  
- Digital data reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2015/ASK%20demodulation%20using%20Envelope%20detector%20Output.jpg" />
</div>

### Introduction





</details>

<details>
<summary> Experiment 16 - Frequency Shift Keying(FSK) </summary>

### Objectives

- Understand the principle of Frequency Shift Keying modulation

- Implement an FSK modulator circuit

### Introduction

Frequency Shift Keying (FSK) works by changing the carrier frequency based on digital data. Logic 1 is represented by one frequency (mark frequency), while logic 0 is represented by another frequency (space frequency). The amplitude remains constant throughout, making FSK more noise-resistant than ASK.

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2016/FSK%20Demo.JPG" />
</div>

### Block diagram

- FSK Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2016/FSK%20Generation%20BD.JPG" />
</div>

A voltage-controlled oscillator (VCO) produces two frequencies controlled by the digital input. HIGH input generates a higher frequency; LOW input generates a lower frequency, producing a continuous waveform that changes frequency with the data.
  
- Digital signal reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2016/FSK%20Restoration%20BD.JPG" />
</div>



### Setup

- FSK Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2016/FSK%20Generation%20setup.jpg" />
</div>

- Digital signal reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2016/FSK%20restoration%20setup.jpg" />
</div>

### Output

- FSK Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2016/FSK%20Output.jpg" />
</div>

- Digital signal reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2016/FSK%20Restoration%20output%20comparison.jpg" />
</div>

</details>

<details>
<summary> Experiment 17 - Binary phase shift keying(BPSK) </summary>



### Objectives

- Understand the principle of Binary Phase Shift Keying modulation

- Implement a BPSK modulator circuit

- Observe how binary data is represented by phase changes in the carrier

### Introduction

Binary Phase Shift Keying (BPSK) works by shifting the carrier phase by 180 degrees according to digital data. Logic 1 is transmitted with 0° phase, while logic 0 is transmitted with 180° phase. The amplitude and frequency remain constant, with information carried entirely in phase changes.

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Additional%20data/Experiment%2017/BPSK%20Demo.JPG" />
</div>

### Block diagram

- BPSK Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2017/BPSK%20Generation%20BD.JPG" />
</div>

The block diagram illustrates how phase reversals encode digital information using the EMONA modules. Master signals  generates a constant carrier sine wave at a fixed frequency. This carrier is fed into one input of a Balanced Modulator or Multiplier module. The  Sequence Generator module produces the binary message signal, but unlike in ASK, this digital signal must be converted to a bipolar format where logic 1 becomes a positive voltage and logic 0 becomes a negative voltage of equal magnitude. This is typically achieved using a Level Converter or by using the digital signal to control an analog switch that selects between +V and -V references. This bipolar digital signal is applied to the second input of the Balanced Modulator. The multiplier performs analog multiplication: when the digital signal is positive, the carrier passes through with its original phase (0° reference); when the digital signal is negative, the multiplication effectively inverts the carrier, producing a 180° phase shift.


- BPSK Demodulation

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2017/BPSK%20Demodulation%20BD.JPG" />
</div>

The incoming BPSK signal is multiplied by a synchronized local carrier in a Product Detector module. This multiplication produces a baseband signal representing the original data plus high-frequency components. A Tunable Low-Pass Filter removes the high-frequency content, leaving a bipolar analog waveform that swings positive and negative corresponding to the original data.

- Digital message reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2017/BPSK%20Digital%20message%20restoration.JPG" />
</div>

The bipolar baseband signal from the filter is fed into a Comparator with its threshold set to zero volts. When the signal is positive, the comparator outputs logic 1 when negative, logic 0. This reconstructs the original digital data, though phase ambiguity may occur if the local carrier is 180° out of phase.



### Setup

- BPSK Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2017/BPSK%20Setup.jpg" />
</div>
	
  
- BPSK Demodulator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2017/BPSK%20demodulation%20setup.jpg" />
</div>

- Digital message reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2017/BPSK%20Digital%20data%20restoration%20setup.jpg" />
</div>


### Output

- BPSK Generator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2017/BPSK%20Generation%20output.jpg" />
</div>

- BPSK Demodulator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2017/BPSK%20demodulation%20output.jpg" />
</div>

- Digital message reconstruction

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2017/BPSK%20Digital%20data%20restoration%20output.jpg" />
</div>

  
</details>

<details>
<summary> Experiment 18 - Quadrature Phase Shift keying(QPSK) </summary>

### Objectives

- Understand the principle of Quadrature Phase Shift Keying modulation

- Learn how to separate digital data into even and odd bit streams using serial-to-parallel conversion

- Implement a QPSK modulator using quadrature carriers

### Introduction

Quadrature Phase Shift Keying (QPSK) works by transmitting two bits per symbol using four phase states. The incoming serial data is split into even and odd bit streams. Even bits modulate an in-phase carrier (cos), while odd bits modulate a quadrature carrier (sin) that is 90° shifted.

### Block diagram

- QPSK Even or odd bits(input signal) setup
  
<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2018/QPSK%20signal%20recovery%20BD.JPG" />
</div>

A Serial-to-Parallel Converter splits the incoming high-speed serial data into two parallel streams: even bits go to the in-phase (I) channel and odd bits go to the quadrature (Q) channel. Both streams pass through level converters that transform standard logic levels into bipolar signals (+V for 1, -V for 0) required for modulation. Each stream now runs at half the original bit rate.

- QPSK Generation

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2018/QPSK%20BD.JPG" />
</div>

A master carrier from an Audio Oscillator is split into two paths. One path goes directly to a Balanced Modulator for the I channel (cos carrier). The second path passes through a 90° Phase Shifter to a second modulator for the Q channel (sin carrier). The I data modulates the cos carrier, the Q data modulates the sin carrier, and an Adder combines both outputs. 
  
- Digital data recovery

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2018/QPSK%20Even%20or%20odd%20bits%20BD.JPG" />
</div>

The incoming QPSK signal is split and fed to two Product Detectors. One detector uses a recovered in-phase carrier (cos) to recover the I data, while the other uses a quadrature carrier (sin) to recover the Q data. Low-pass filters remove high-frequency components, and Comparators regenerate clean I and Q digital streams.

### Setup

- QPSK Even or odd bits(input signal) setup

<div align="center">
<img width="500" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2018/Digital%20data%20input%20setup.JPG" />
</div>

- QPSK Generation

<div align="center">
<img width="1000" height="1500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2018/QPSK%20Setup.JPG" />
</div>

  
- Digital data recovery

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2018/QPSK%20signal%20demodulation%20setup.JPG" />
</div>
  
### Output

- QPSK Even or odd bits(input signal) setup

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2018/digital%20data%20output.JPG" />
</div>

- QPSK Generation

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2018/QPSK%20Output.JPG" />
</div>

- Digital data recovery

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2018/QPSK%20X1%20Reconstruction.JPG" />
</div>

</details>

<details>
<summary> Experiment 19 - DSSS Modulation and Demodulation </summary>

- To understand the principle of Direct Sequence Spread Spectrum modulation

- To implement a DSSS modulator using a PN sequence generator on the EMONA trainer

### Objectives

### Introduction

Direct Sequence Spread Spectrum (DSSS) works by multiplying digital data with a high-rate pseudo-random noise (PN) sequence. This spreads the signal energy over a much wider bandwidth, making it appear noise-like. The receiver uses an identical synchronized PN sequence to despread the signal, recovering the original data while suppressing interference and jamming. The processing gain, determined by the ratio of spreading bandwidth to data bandwidth, provides resistance to narrowband interferers.

### Block diagram

- DSSS Modulator and demodulator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2019/DSSS%20Modulator%20and%20Product%20detector%20BD.JPG" />
</div>

A Digital Sequence Generator provides low-rate data to a Multiplier, while a Pseudo-Random Noise (PN) Sequence Generator provides a high-rate chipping sequence to the multiplier's other input. This multiplication spreads the signal over a wide bandwidth. The spread signal modulates a carrier using another multiplier. At the receiver, the same synchronized PN sequence multiplies the incoming signal to despread it, collapsing it back to narrowband while spreading any interference. A product detector and filter recover the original data.

- DSSS with channel signal jammer

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2019/DSSS%20Modulator%20and%20demodulator%20with%20jamming%20signal%20BD.JPG" />
</div>

This extends the basic system by adding a jamming signal generator (Audio Oscillator or VCO) that feeds into an Adder along with the transmitted DSSS signal. The adder combines both signals to simulate a noisy channel. At the receiver, despreading spreads the jammer's energy over a wide bandwidth while despreading the desired signal. Subsequent low-pass filtering removes most of the jammer energy, demonstrating DSSS interference rejection. The processing gain determines how much rejection is achieved.

### Setup

- DSSS Modulator and demodulator

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2019/DSSS%20Modulation%20and%20demodulation(product%20detector)%20setup.JPG" />
</div>
  
- DSSS with channel signal jammer

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2019/DSSS%20Modulation%20and%20demodulation%20with%20signal%20jamming%20setup.JPG" />
</div>

### Output

- DSSS Modulator and demodulator

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2019/DSSS%20Modulation%20and%20demodulation%20output%20comparison.JPG" />
</div>

  
- DSSS with channel signal jammer

 If Adder gain for signal jammer is low under low frequency

<div align="center">
<img width="1000" height="1000" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2019/Low%20adder%20gain%20Signal%20jammer%20VCO%20at%20low%20frequency.JPG" />
</div>

 If adder gain for signal jammer is low under high frequency

 <div align="center">
 <img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2019/Low%20adder%20gain%20Signal%20jammer%20VCO%20at%20high%20frequency.JPG" />
 </div>

  If Adder gain for signal jammer is high under low frequency

  <div align="center">
  <img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2019/High%20adder%20gain%20Signal%20jammer%20VCO%20at%20low%20frequency.JPG" />
  </div>

  If Adder gain for signal jammer is high under high frequency

  <div align="center">
  <img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2019/High%20adder%20gain%20Signal%20jammer%20VCO%20at%20high%20frequency.JPG" />
  </div>

</details>

<details>
<summary> Experiment 20 - Understanding in software defined radio </summary>

### Objectives

- To understand the basic concepts of Software Defined Radio

- To learn about undersampling and its application in SDR receivers

### Introduction

Software Defined Radio (SDR) works by moving analog-to-digital conversion as close to the antenna as possible and performing signal processing in software. This experiment demonstrates undersampling, where sampling below the Nyquist rate causes controlled aliasing that folds modulated signals down to baseband. This technique replaces traditional mixing stages with digital processing, illustrating how the same hardware can handle different modulation types by simply changing the software.

### Block diagram

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Block%20diagrams/Experiment%2020/Undersampling%20DSBSC%20Signal%20%20BD.JPG" />
</div>

A DSBSC signal is generated using an Audio Oscillator (message) and another oscillator (carrier) feeding a Balanced Modulator. This DSBSC signal is connected to a Sampler module controlled by a sampling pulse train. The sampling frequency is deliberately set below the Nyquist rate for the carrier, causing undersampling that folds the modulated signal down to baseband through aliasing. A Tunable Low-Pass Filter then selects the baseband component, effectively demodulating the signal without traditional mixers. Replacing the fixed sampling signal with a VCO makes the system tunable, demonstrating the SDR principle of moving digitization close to the antenna and performing frequency conversion through digital techniques.

### Setup

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2020/DSBSC%20Modulation%20and%20demodulation%20setup.JPG" />
</div>

  
- Replace samplig signal with VCO

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Setup/Experiment%2020/DSBSC%20sampling%20modification%20setup.JPG" />
</div>

### Output

<div align="center">
<img width="500" height="500" alt="image" src="https://raw.githubusercontent.com/dexterestacion/NEC-4203-LAB-REPORT-3/refs/heads/main/Output/Experiment%2020/DSBSC%20demodulation%20output.JPG" />
</div>

</details>

<details>
<summary>Reference</summary>
  
### Experiment 9
  
  - https://blog.truegeometry.com/api/exploreHTML/42c699040c9d7b230a38fff56c680c96.exploreHTML
  - https://electronicscoach.com/frequency-modulation.html
  
### Experiment 10
  - https://user.eng.umd.edu/~tretter/commlab/c6713slides/ch8.pdf
  - https://ae-iitr.vlabs.ac.in/exp/voltage-comparator/theory.html
    
### Experiment 11
  - https://uomus.edu.iq/img/lectures21/MUCLecture_2025_225463.pdf
    
### Experiment 12
  - https://www.sciencedirect.com/topics/engineering/pulse-code-modulation
  - https://www.eng.auburn.edu/~troppel/courses/TIMS-manuals-r5/TIMS%20Experiment%20Manuals/Student_Text/Vol-D1/D1-11.pdf
  - https://byjus.com/physics/pulse-code-modulation/
    
### Experiment 13
  - https://www.egr.msu.edu/classes/ece458/radha/ss07Keyur/Lab-Handouts/Lab9PCM.pdf
  - https://ecedunia.blogspot.com/2016/03/pulse-code-modulation.html
  - https://codes.pratikkataria.com/communication-system/

 ### Experiment 14
 
 ### Experiment 15
 
 ### Experiment 16
 
 ### Experiment 17
 
 ### Experiment 18
 
 ### Experiment 19
 - https://webstor.srmist.edu.in/web_assets/srm_mainsite/files/files/lab_experiment.pdf
   
 
 ### Experiment 20
 

  
</details>
