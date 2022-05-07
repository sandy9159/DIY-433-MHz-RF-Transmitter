# DIY-433-MHz-RF-Transmitter

![image](https://user-images.githubusercontent.com/19898602/167255213-d5ad9cb5-e7e1-4ed5-aef6-588ce95f393c.png)


An RF Beacon is a circuit that produces a continuous pulse that helps with tracking down an item or vehicle. One use for such a beacon would be to locate a rocket when it comes back down too far away to be seen. In this DIY Hacking project, 

we will use a 433 MHz RF transmitter and a pair of 555 astable oscillators to create an RF beacon.


![image](https://user-images.githubusercontent.com/19898602/167255228-dab59d37-a61f-4136-9632-88375d80082f.png)


# Component Required

![image](https://user-images.githubusercontent.com/19898602/167255297-c7e04c0f-460a-4d25-b972-e57f7cc81231.png)

1KΩ Resistor (R5, R6, R7)
10KΩ Resistor (R1, R3, R4, R8)
100KΩ Resistor (R2)
10nF Capacitor (C2, C3, C4)
10uF Capacitor (C1)
2N3904 (Q1, Q2)
555 Timer (IC1, IC2)
RF Module (433 MHz)


# RF Beacon Circuit Schematic

![image](https://user-images.githubusercontent.com/19898602/167255347-084623f6-5727-4e8b-9db7-687e71f12fd5.png)


# How Does it Work?

The RF beacon consists of three main units; A low frequency 555 oscillator, an audio (high frequency) oscillator, and an RF 433MHz module. The first unit, a low-frequency oscillator, creates a pulse at a frequency of approximately 1Hz which has an extremely large duty cycle (close to 99.9%).

This signal is then inverted thanks to Q1 in the form of a NOT gate, this creates a pulse with a duty cycle near 0.01%. The low duty cycle pulse is connected to the RESET of an audio 555 oscillator. When the output from the low-frequency oscillator stage (after Q1) becomes 0V, the audio oscillator (IC2), 

is disabled and the result is no audio signal being produced. When the output of the low-frequency oscillator becomes VCC then the audio oscillator (IC2) is enabled and produces an audio able tone. This signal is inverted and then fed into the RF module which emits a tone on the 433MHz spectrum which can easily be picked up by receivers.

# Constructing Your RF Beacon

The circuit can be built using through hole techniques including PCB, solderless breadboard, stripboard, and even matrix board. While the circuit shown here is rather large, it can easily be shrunk down using surface mount components. 

That way, the circuit can easily be fitted onto small drones and RC planes while also keeping weight down to add RF tracking capabilities. For this project, a custom PCB has been designed to demonstrate the circuit using CNC milling. 

All the files needed for this project can be found here including the CNC code needed to make the PCB: RF Beacon Project Files.

The Idea I get from https://maker.pro/pcb/projects/rf-beacon-build-433-mhz-rf-transmitter

then I Decide to make it'S PCB version also and share with you guys, so you can find the PCB files below



# Custom PCB for RF Beacon Circuit




![image](https://user-images.githubusercontent.com/19898602/167255414-dfe45fea-f6fc-4a38-a1b3-2ea91afc0595.png)

![image](https://user-images.githubusercontent.com/19898602/167255424-1f789500-42de-4122-ab77-3e1e88239864.png)

![image](https://user-images.githubusercontent.com/19898602/167255442-98c056ab-a316-497f-b14e-e0f42e9caf42.png)


You can download and modify the PCB by visiting the link below









