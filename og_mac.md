# PicoPSU Adaptor for Macintosh 128K / 512K / Mac Plus

[Purchase Link](https://www.tindie.com/products/28754/) | [Official Discord](https://discord.gg/HAuuh3pAmB) | [Table of Contents](#table-of-contents)

----

This adaptor lets you use **Pico ATX PSU** in Macintosh 128K / 512K / Plus computers.

It plugs into the motherboard and bypasses the unreliable internal PSU all together.

![Alt text](photos/mac_plus/title.jpg)

## Features

* **Non-destructive** and reversible

* **PC fan header** for added cooling

* Universal voltage with fused rails

* Low cost, efficient and reliable.

## Get One / Other Stuff

[Click me to get one!](https://www.tindie.com/products/28754/)

Also available for [Compact Macintosh, Apple IIGS, BBC Micro, Osborne 1, and more!](./README.md)

For more general-purpose diagnostics and retrofitting, check out the [full-fat ATX4VC](https://github.com/dekuNukem/ATX4VC)!

## Table of Contents

- [Getting a Pico PSU](#getting-a-pico-psu)

- [Kit Assembly](#kit-assembly)

- [Installation](#installation)

- [Troubleshooting](#troubleshooting)

- [Questions or Comments?](#questions-or-comments)

## Getting a Pico PSU

PicoPSU are tiny ATX power supplies for small PCs, but perfect for retro computers as well.

![Alt text](photos/mac_plus/pico.jpg)

* [Official website](https://www.mini-box.com/DC-DC) and [distributors](https://www.mini-box.com/site/resellers.html). Even the cheapest 80W one should be plenty.

* Avoid generic clones. They over-rate and are of low quality.

* A power brick with **12V DC** and **center positive** 5.5x2.5mm barrel jack is needed.

* Those are very popular and you might already have one. Make sure it has enough wattage.

Remember that this solution is **only as good as your PicoPSU and 12V Brick**, so don't skimp on them!

## Kit Assembly

**DON'T START YET!!!** Keep reading :)

### Soldering Notes

Nothing too tricky in this kit, all basic through-hole stuff.

If this is your first time, a few tips:

* Make sure your soldering iron has **proper temperature control**. Try your local makerspace or university lab.

* Use **leaded solder** and plenty of flux, temperature around 320C / 600F.

* [This video](https://www.youtube.com/watch?v=AqvHogekDI4) covers the basics pretty well.

* Start from shortest to tallest. Solder **a single pin** first, and make sure the part is straight.

### Assembly

Parts are slightly different for Mac Plus and Mac 128K/512K, make sure to follow the correct one!

![Alt text](photos/mac_plus/macplus_parts.png)

![Alt text](photos/mac_plus/macog_parts.png)

Solder the components **as shown below**:

![Alt text](photos/mac_plus/assnote.png)

* Double check capacitor polarity!

* Black electrolytic caps: White stripe is **NEGATIVE**.

* Blue Tantalum caps: White stripe is **POSITIVE**.

* Yellow ceramic caps: No polarity.

### Cleaning

This is optional, but I like to clean off the flux with 90%+ isopropyl alcohol. Submerge and scrub with a toothbrush.

Make sure it is **completely dry** before proceeding.

### Inspection

* Compare with the reference photo and notes, make sure everything is in correct orientation.

* Solder joints should be **shiny and smooth**. If you see spikes, put on more flux and melt it again.

* There must be **no solder bridges**. If any, put on flux and melt it to remove.

![Alt text](photos/mac_plus/macplus_ref.png)

![Alt text](photos/mac_plus/macog_ref.png)

## Board Features

Install the fuses.

![Alt text](photos/mac_plus/features.png)

### Power Switch

The PSW pin header is connected to the ATX `PS_ON` pin.

You can wire a latching switch to it, or leave it jumpered so it turns on immediately when plugged in.

### PC Fan Header

* Any standard 3 or 4-pin PC fan should work

### Fuse

* Use common car fuse RATED **5A OR LESS**

* Regular, Mini, and low-profile Mini all will work. Simply push into the holder.

* **DO NOT BYPASS FUSES**

### Battery Header (Optional)

* You can connect a backup battery to the header.

## Pre-installation Checks

From the back, use a multimeter to **check for dead shorts** between each power pin and GND:

![Alt text](photos/mac_plus/short.png)

If all good, plug in Pico ATX PSU, and then power jack.

The PSU should turn on, measure the voltage on each rail and confirm they are within spec.

## Installation

During disassembly, it's a good idea to **take plenty of photos**. It never hurts to have reference.

### Remove Back Cover

⚠️**Dangerous CRT voltage inside**! Make sure the computer is **unplugged for a few hours**! Or discharge the CRT yourself.

You'll need a LONG **Torx T15 screwdriver**.

Recommended steps:

* Lay the Mac face down on a soft cloth

* Loosen all screws. Two at the bottom, one behind battery door, two in the handles.

* Remove all screws **APART FROM a single one inside the handle**.

* Take photos of which goes in where, the lower two has a thinner thread.

![Alt text](photos/mac_plus/back.png)

* Put the screwdriver on that single loosened screw.

* Push down on it while **gently** lifting up the back cover. It should pop loose.

* Slowly **lift straight up** to remove the back cover.

![Alt text](photos/mac_plus/backoff.gif)

⚠️ **DO NOT TOUCH ANY CRT COMPONENTS** if you don't know what you're doing!

### Install the Adaptor

* Unplug the floppy and power cable from motherboard.

* **DO NOT YANK STRAIGHT UP**, or you might break the CRT neck!

* Wiggle gently until loose, and carefully unplug.

![Alt text](photos/mac_plus/11p.jpeg)

* Plug the Pico PSU and the power cable into the adaptor.

* The missing wire should match the missing pin on the socket.

![Alt text](photos/mac_plus/cable.jpeg)

* **[MAC PLUS]** Plug the adaptor back into the motherboard.

![Alt text](photos/mac_plus/macplus_mb.jpeg)

* It should go in firmly, although not reach the bottom.

* **Bend down and double check from both sides** that the pins are lined up and NOT off-by-one!

![Alt text](photos/mac_plus/off1.png)

* **[MAC 128K/512K]** Plug the extension cable into motherboard, then into bottom of the adaptor.

* Again, make sure the **missing wire matches the missing pin** on the socket.

![Alt text](photos/mac_plus/128k.jpeg)

*I don't have a Mac 128K so this will have to do*

* The adaptor will be floating in mid-air, which is unfortunate. Still, make sure it does not short on other components or metal case, secure and add insulation if needed.

### Moment of Truth!

If everything checks out, take a breath and plug it in.

If your Mac was working before, hopefully it still does!

If the Mac is of unknown condition, now you'll find out!

![Alt text](photos/mac_plus/working.jpeg)

And if it doesn't work, [check out the troubleshooting guide](#troubleshooting). 

### Big Mac Fan

Early Macs run really hot, so it's a good idea to put in a fan.

Any PC case fan should work.

Vents on top of the case is a good location, maybe you can ziptie it there. Of course it's up to you!

Make sure the fan is secured, nothing touches the blade, and air flow direction is correct.

**Don't mount the fan too close to the CRT**, or the picture might wobble from the motor's magnetic field.

## Power Routing

Now it works, how are we going to mount the DC jack receptacle?

I'll admit this is where things goes a bit downhill, as there doesn't appear to be a way that's **BOTH non-destructive AND elegant**.

Neat but destructive: Just drill a hole. **DO NOT DO THIS!**

Non-destructive but a bit messy: Extend the power cable though the case.

I'll cover the second route.

---

Cut the power cable in half:

![Alt text](photos/mac_plus/half.jpeg)

Now we're going to add some extra length.

You can solder it, but I highly recommend using lever connectors such as the ones from WAGO.

Strip the cables to the marked length, flip up, insert, flip down. Make sure the colors match.

![Alt text](photos/mac_plus/strip.jpeg)

![Alt text](photos/mac_plus/extra.jpeg)

Now thread the cable through the square hole on the battery holder.

![Alt text](photos/mac_plus/route.jpeg)

Thread it though the same hole on the back case, now you can put it back on.

Connect the other end in the same way.

![Alt text](photos/mac_plus/back.jpeg)

**Insert the blanking plug** to prevent accidentally energizing the old PSU and blow everything up.

![Alt text](photos/mac_plus/plug.jpeg)


Now you just have to plug in the DC jack to turn it on.

There is definitely room for improvements here, so if you come up with anything [let me know](#questions-or-comments) and I'll update it!

A few ideas:

* Just wire in an in-line switch.

* Desolder the original IEC connector and mount the jack there?

* Maybe wire the built-in power switch to the PSW header? Might need to cut traces.

## Enjoy!

With internal PSU bypassed and added cooling, may your Mac lives many more years of trouble-free life!

![Alt text](photos/mac_plus/final.jpeg)

What's with the wireless keyboard and mouse? [Check out USB4VC!](https://github.com/dekuNukem/USB4VC/blob/master/README.md)

Questions or comments? Ask in our [Discord](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/ATX4VC/issues), or email `dekunukem` `gmail.com`!

## Troubleshooting

This adaptor eliminates the PSU from the equation, but that's only part of the puzzle!

If something else is wrong, you still need to fix it.

### Nothing Happens

* Check for shorts on power rails, you can measure it on the back of analog board after removing the paper insulation.

![Alt text](photos/mac_plus/pinout.png)

* [This document](resources/plus_analog.pdf) is very helpful for finding faults on the analog board.

* Check fuse

### CRT Geometry Messed Up

I had this happen with a knock-off generic PicoPSU, changing to another one fixed it.

### Screen Wobbles

* If it happens when floppy drive is active, try using a beefier power brick, or add more decoupling capacitors.

* If happens while idle, make sure the fan is not too close to the CRT.

### Other Failures

Other common issues include:

* Cracked solder joints

* Shorted tantalum capacitors

* Dirty contacts / Bad RAMs

I highly recommend watching [Adrian's Digital Basement Macintosh Repair-a-thon](https://www.youtube.com/watch?v=lKD65I86XGQ), where he covers a lot of those in detail.

The **power connector** and CRT **deflection capacitors** are notorious for cracking, here are some examples on mine:

![Alt text](photos/mac_plus/crack1.jpeg)

![Alt text](photos/mac_plus/crack2.jpeg)

It might be very difficult to see with naked eye, so use magnification!

Flux and new solder should fix it right up, if you find one crack might as well do the whole row.

## Questions or Comments?

Feel free to ask in official [Discord Chatroom](https://discord.gg/T9uuFudg7j), raise a [Github issue](https://github.com/dekuNukem/PicoRC/issues), or email `dekunukem` `gmail.com`!
