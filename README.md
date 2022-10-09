# Integrated Circuit(IC) Model

This repository presents the design of Integrated-Circuit(IC) Model implemented using eSim open source EDA tool.

# Table of Contents

- [Abstract](#Abstract)
- [Introduction](#Introduction)


# Introduction

FOSSEE (Free/Libre and Open Source Software for Education) project promotes the use of FLOSS tools to improve the quality of education in India. It aims to reduce dependency on proprietary software in educational institutions. It encourages the use of FLOSS tools through various activities to ensure commercial software is replaced by equivalent FLOSS tools. It also develops new FLOSS tools and upgrade existing tools to meet requirements in academia and research \cite{paknikar2021esim}.
The FOSSEE project is part of the National Mission on Education through Information and Communication Technology (ICT), Ministry of Human Resource Device modelling is one area where measurement and EDA have long collaborated well. The correctness of designs is crucial because they are constructed from device models.
However, models are only as good as the measured data that was used to generate them, therefore measurement is essential to obtaining precise and useful device data for modelling \cite{} In order to simulate the behaviour of the individual components, they have to be described mathematically. The equations that describe diodes, bipolar (bjt) and a variety of field effect (jfet) and MOS transistors become increasingly complex, sometimes with several equations describing the behaviour of different aspects of device performance in different regions of operation. Different sets of equations may be used to describe devices in the same family of devices, such as MOSFETs, because these sets of equations are heavily depending on the semiconductor physics of devices and the fabrication procedures used to make them. The producer may utilise several sets of equations in order to more accurately or less accurately describe how their products function.In general, the coefficients of the sets of equations are gathered together in the form of a list, even though the equations themselves are deeply buried in a simulator's source code. A list of coefficients, known as a model, can then be used to characterise each individual device in a given device family. The individual coefficients in a model are called the model parameters.


# Analog integrated circuit

Analog integrated circuit design are those which are used for designing operational amplifiers, linear regulators, oscillators, active filters, and phase locked loops. And for verifying the semiconductor parameters like power dissipation, gain, and resistance which is more concerned while designing the analog integrated circuit.
Analog Integrated Ic's are used for performing different operations on analog signals. As, we all know that analog signals are present everywhere in nature. So, to perform different operations we use analog IC's.

Different types of Analog Ic's are opamp 741 Ic,LM386,cd4017,etc.

## INA106 Differential Amplifier IC

Differential Amplifier is a type of amplifier circuit which is used to amplify the difference of input and give the output respectively.

### Pin Configuration

It is an 8 pins IC \cite{6} with pin name REF, -IN, +IN , V- , Sense , Vout , V+ , NC.  It is an analog circuit which takes two input and give the difference of both inputs at the output.

</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/194776865-56133d90-b082-449a-8c25-cc44b4dd8114.jpg"></br>
   fig.1: INA106 Pin Configuration 
</p>

The mathematical equation for calculating the output is given as
Vout=Ad(Vin1-Vin2)
Where,
Vin1 = it is the voltage applied at the inverting terminal of op-amp
Vin2= it is the voltage applied at the non-inverting terminal of op-amp
Ad= Differential Gain
Vout= It is the output of the op-amp.
• To calculate the differential amplifier gain we can use :-
Ad=Vout/(Vin1-Vin2)


### Subcircuit Schematic Diagram


</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/194777014-3fed0704-346b-40a3-b787-04e01139257c.jpg"></br>
   fig.2: Subcircuit Schematic Diagram of INA106 Differential Amplifier using OPAMP 
</p>

#### Schematic with external circui


</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/90523478/194777098-27316c0c-6512-4ed1-9853-354622c7da23.jpg"></br>
   fig.3: Schematic of differential amplifier 
</p>
