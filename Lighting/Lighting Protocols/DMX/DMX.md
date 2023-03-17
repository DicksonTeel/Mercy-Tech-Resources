**DMX stands for Digital Multi-PleXing, and it refers to the DMX512 spec, which means 512 channels in a universe**

# The Universe
512 channels of control — this means you can control up to 512 different functions spread across whatever number of light fixtures, smoke, or effects fixtures you are running. If you need more than 512, then you will need to use additional universes.

# How it Works
Each DMX capable fixture gets assigned an ID/address and it uses as many channels to control its functions as it needs. Ideally, each fixture has a unique DMX ID/address, although any fixtures that have the same ID/address will react to the same commands. Every DMX fixture has an input and an output, allowing you to daisy-chain your DMX cable from one light to the next. Just make sure to give each fixture a discrete DMX address for individual control. DMX is robust, and has been around since 1986 for the simple reason that it works.

## Wait a Bit; is it 8- or 16-Bit?
DMX sends an 8-bit “word” for each function, this generally provides 256 steps of control per channel. If this is not smooth enough as you dim your fixture, for example, some fixtures support a 16-bit mode that will use two channels; one for coarse adjustment and one for fine adjustment.

# Consoles
In the end, a lighting console (whether a physical board or computer software) is what you need to control your fixtures, and the capabilities of your board will define what you can do. While a DMX Universe is up to 512 functions, not all consoles will support that.

# What Can Go Wrong?
DMX is simple and robust, so very little can go wrong, but that doesn’t mean it can’t fail. Read on for some useful suggestions to avoid catastrophe:

## Use a Terminator, or Your Signal Just May Say, “I’ll Be Back”
First, you need a terminator for the DMX signal. Without a signal terminator, your DMX signal will reach the end of the line, and bounce back like a rubber ball off a wall. This is known as a reflection and it will interfere with your DMX signal. Those of you who remember analog video monitors may recall what happened when you forgot to terminate the video signal — you saw a very distorted signal on your monitor. At some point, monitors became auto-terminating and worked very well, and we no longer had to carry terminating BNC connectors to pop onto the monitor’s video out.

Auto-termination is still pretty new on DMX fixtures and can be imperfect. A simple terminator on the output of the last fixture in the chain will help prevent the signal from reflecting and traveling back down the chain, causing interference that will affect the smooth operation of your fixtures. Even if the fixture is self-terminating, adding a terminator can’t hurt. (If you wish to build your own, DMX Terminators utilize a 120 Ohm resistor)

## Cables: it’s Digital and it Matters
The DMX protocol calls for 5-pin XLR connectors and low capacitance cable. You may see fixtures that sport 3-pin connectors or even RJ45 (Ethernet) connectors for DMX. The concern with 3-pin XLR connectors is that they are commonly used for mic cables, which may lead you to think that you can use mic cables. However, most mic cables are high-capacitance. Capacitance may not cause a problem for analog audio signals, but it certainly does affect digital signals. DMX signals are a square wave, and the space between the signals is very important. High-capacitance cables will degrade the signal, because they absorb some of the power within the signal, transforming the nice, clean square wave signal into a saw-tooth signal that may not work properly. So, don’t use mic cables. No matter which connector you are using, you need to use low-capacitance cables.

### Distance
So, how long can your cable run be? The DMX specification states the maximum length is 3,281'—but think about it. We are working in the real world; every connection can degrade the signal. A good working practice is to limit your cable run to 1,000'.

## Number of Units
32 “loads” is the practical limit. A load is basically a light or effects fixture, and it doesn’t matter how many or how few channels that fixture uses. Could your DMX setup work with 33 or more loads? Probably, but will it be reliable? Why risk it? A simple data splitter comes in handy here. This is not just a simple Y-cable—don’t use a Y-cable, because it introduces noise and splits the signal, weakening it. Always use a data splitter. A data splitter is also useful for extending cable runs longer than 1,000'.