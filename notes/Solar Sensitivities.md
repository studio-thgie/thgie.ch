---
title: Solar Sensitivities
---
# Solar Sensitivities [^1]
This is the base note for a new line of inquiry that grew out of a reflection on what to do with my own practice in these times of crisis. I'm very much invested into technology, especially digital ones. The last 10 to 50 years have shown, that our collective imagination of technology does a lot of harm to the planet, to flora and fauna, and to ourselves. Harm that would not be necessary and which by far outweights the good. Solar Sensitivities then is an attempt to bring my own practice into accordance with my values.

## Solar-powered server
This is the original inspirational document by low-tech magazine: [How to build a Low-Tech website: Software & Hardware](https://homebrewserver.club/low-tech-website-howto.html). The easiest solution… is probably to just buy the PiJuice shield and solar panel. But it feels a bit to quick. I would love to learn just a bit more about electricity. Pidora has a good step by step over view on [how to build a solar powered raspi server](https://pidora.ca/how-to-build-a-solar-powered-raspberry-pi/). The shield has the ability to safely turn on and off the device. [This article by active countermeasures](https://www.activecountermeasures.com/making-a-solar-powered-raspberry-pi/) (🙄) opts for the USB powerbank, which I also like.

*How much power does a raspi w/o desktop need?*

### Research on Raspberry Pi and Batteries
So it seems a [raspi 4 needs between 2.7 to 3.4 W](https://www.pidramble.com/wiki/benchmarks/power-consumption). [Core electronics has a good primer](https://core-electronics.com.au/tutorials/solar-powered-pi.html#Size) on how much energy is needed and how much is produced. The biggest PiJuice solar panel produces 44W, whereas the low-tech magazine setup has a 50 Wp (?) panel.

I have to ask a specialist (Ramon ;)) on how some of the details work. Does the solar panel charge battery pack and server at the same time? Did I get all of the watt[^2], watt-hour, ampere things right? 

- Batterypower and solarpanel calculations
	- [https://www.youtube.com/watch?v=lPyDtuzYE5s](https://www.youtube.com/watch?v=lPyDtuzYE5s)
	- [https://www.youtube.com/watch?v=TJBGbufexEM](https://www.youtube.com/watch?v=TJBGbufexEM)

### How to setup a solar panel…
The cable that come out of the panel look weird.

## Journal
### Update 2022-05-09
I bought myself a large panel (110W) and an easy MPPT. That is a little thing that stabilises the energy that comes out of the panel. Because the sun-shine fluctuates, and with it the energy-current, it can be problematic for the things you attach to the panel. This particular MPPT by revolt[^3] also has USB outlets, which is nice. If it produces to much power, maybe we can even charge some other devices.

I do need to learn how to set up the panel now, and if I miss anything… Oook I was missing a few things.

- an MPPT should not be setup without a battery hooked up to it. That could damage the MPPT. So I had to order a battery as well
- The cables that came out of the solar panel are the MC4 type. I did order proper cables into the MPPT, but they lack the MC4 adapters on the other end, so I had to order that as well.

## Foundation
- [How to Build a Low-tech Website?](reading/@HowBuildLowtech2018.md)

## Inspiration and entanglements
- [Solar Protocol](http://solarprotocol.net/[**[]()**]())
- [uxn](https://compudanzas.net/uxn_tutorial.html)
- [LIMITS conference](https://computingwithinlimits.org/2022/)
- [100r](http://100r.co/site/home.html)
- [low carbon research methods](http://lowcarbonmethods.com/index.html)
- [the intersection, by superflux](https://superflux.in/index.php/work/the-intersection/#)
- [DIY Methods 2022 Conference](https://www.diymethods.net/)

[^1]: Will the title hold? We will see. But it's poetic, and I like it. I could spin a whole theme around it.
[^2]: https://www.electricityforum.com/what-is-a-watt
[^3]: https://www.revolt-power.de/Digital-Solar-Laderegler-20A-12V-24V-Auto-Switch--NX-6816-919.shtml