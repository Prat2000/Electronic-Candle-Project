# FLAMELESS SMART ELECTRONIC CANDLE 
## Description
Candles are a source of light and warmth as well as a good decorative stuff that all of us are familier with.But the wax candles we use have a short life as they melt away and also require great caution while handling.<br>
A smart solution to this is **An Electronic Candle**.<br>
The electronic candle uses light sensors which detect variation in light intensity in the surrounding.It automatically switches **ON** in low-lit conditions and switches **OFF** in lighted conditions. 
## Materials Required
1. LM358 IC
2. LDR(Photo Resistor)
3. Resistors: 1M ohm and 1K ohm
4. LEDs
5. 10K Pot(Potentiometer)
6. 12V Battery
7. Breadboard
8. Connecting Wires
## Circuit Diagram

![Circuit](https://user-images.githubusercontent.com/60696998/79799025-74137300-8377-11ea-88c9-6182208f2882.png)

## Working Principle

### LM358 IC
![LM358 IC](https://user-images.githubusercontent.com/60696998/79793717-aa98c000-836e-11ea-9775-d56380407b4c.jpg)<br>

LM358 IC is an Op-amp Comparator IC.It takes in voltages ```Vin+ , Vin-``` through non-inverting terminal (**pin 3**) and inverting terminal (**pin 2**) respectively as inputs, compares them and produces output ```Vout``` in the output terminal (**pin 1**).<br>
The relation is<br>

```Vout = A0( (Vin+) - (Vin-))``` &nbsp;[A0 is the open-loop gain of Op-amp]<br>

**CASE 1 :** When ```Vin+ > Vin-``` then ```Vout``` is **high** .Hence LED switches **ON**.<br>

**CASE 2 :** When ```Vin+ < Vin-``` then ```Vout``` is **low** .Hence LED switches **OFF**.<br>

**NOTE :** In order to calibrate LM358 comparator, adjust the 10K Potentiometer to the level when the LED just turns off. This increases sensitivity of the LDR.

### LDR(Light Dependent Resistor)
![LDR file](https://user-images.githubusercontent.com/60696998/79794328-afaa3f00-836f-11ea-90e9-0eccb448656d.png)<br>

LDR is made up of **Cadmium Sulphide(CdS)** which is a semiconductor material. It is a photo resistor i.e. its resistance depends on incident light intensity.<br>

When the room is dark( or when you cover the LDR with  your hand ), resistance of the LDR is very high( in the range of mega-ohms ) in comparison to the 10K potentiometer. So ```Vin+``` or the non-inverting terminal potential becomes more than ```Vin-``` or the inverting terminal potential. Hence **CASE 1** is satisfied and LED turns **ON**.<br>

When the room is lighted ( or when you uncover the LDR ), resistance of LDR is very low in comparison to the 10K potentiometer.So ```Vin+``` or the non-inverting terminal potential becomes less than ```Vin-``` or the inverting terminal potential. Hence **CASE 2** is satisfied and LED turns **OFF**.<br>

**NOTE :** More than one LEDs can be connected in series for better lighting.
