# FriFilur
Simple Analog Voltmeter Clock powered by batteries called Fri Filur.

The meaning of this repo is to display my clock and to communicate my experience and reflections.

Fri Filur was a simple Arduino project i made in my sparetime in 2019. The result of the project was descent but it has a lot of problems:
1. Power consumption because of the use of the ATMega328p sleep mode is constraint to a higher power consumption mode because of the usage of onboard PWM signals are used for controlling the voltmeters.
2. Through hole soldering on a perf board which is not ideal.
3. A lot of wires cramped into a tight space.
4. Voltmeters are unreliable because the ATMega328p runs on battery power which is inconsistent over time. Recalibration of the meters needs to happen multiple times over the lifetime of the batteries.
5. DS3231 RTC is ot for low power consumption to make it so a lot of changes has to be made.

Even though it had a lot of problems which mainly was focused around the power consumption of the 2xAA batteries it used. It could last for quite some time (But not satisfactorily). They could probably be fixed, either by utilaizing the watchdog timer better (As for PWM)  or by using another breakout or by making it completely hardware based or another way of combining hardware with software is to use a bit shifters for each voltmeter in conjunction with voltage splitters.

The experience throughput when the project was active was through the roof. I still remember the (rather clever i must say myself) solutions to some of my less clever handywork. Eg. how i created a main power connector and fastned the perf board whilst also connecting the voltmeters. The whole fitting work could only be done with slight of hand only seen at the most brilliant magician. The creation breakout boards and learning about the anatomy of the boards really stuck with me. I also learned that i hate tedious cheap chinese wires and that i am not good at deisolating wires. But the thing which really stuck with me is that the plans and schematics i amde for it hardly came to life which sadness me but i came to the conclusion that plans acts more as guides and motivational material than a plan to strictly follow. 

Would i ever create another one? No. But i did have fun.

The main internal contents of the clock:
* ATMega328p breakout soldered to perf board.
* 2AA battery container.
* DS3231 RTC.
* 2 analog voltmeters (10 micro amp).
* Connectors for the voltmeters to the perf board.
* Sarcasme.
