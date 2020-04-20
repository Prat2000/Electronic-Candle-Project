# ELECTRONIC CANDLE PROJECT
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
## Working Principle

### LM358 IC 
LM358 IC is an Op-amp Comparator IC.It takes in voltages ```Vin+ , Vin-``` through inverting terminal (**pin 3**) and non-inverting terminal (**pin 2**) as inputs, compares them and produces output ```Vout``` in the output terminal (**pin 1**).The relation is<br>

```Vout = A0( (Vin+) - (Vin-))```   [A0 is the open-loop gain of Op-amp]
