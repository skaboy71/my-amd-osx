# MY AMD Ryzentosh Project

I had planned on getting a 2019 Mac Pro but since Apple announced the new "apple silicon", I decided to wait till they decide how they're going to bring this architecture to the mix.

In the short-term, my idea was to build myself a linux box as my "daily driver" but after playing with a number of distros I realized I was super dependant on a couple things....... on one thing mainly.  [Alfred](https://www.alfredapp.com/).  There are some "similar" apps for linux but as with most open source, they're not really the "complete solution" that I know, love, and use constantly in Alfred. I can't recommend Alfred highly enough if, like me, you like to automate repettive tasks and have quick elegant access to clipboard history, snippets, and building your orwn custom workflows. 

Due to this, I did some research on ["hackintosh" with AMD](https://amd-osx.com/) and was really suprised to find that it's not only "possible", but that there was a large community of AMD platform users.

I took some time to try and understand the process and managed to get through the ["Vanilla" Install Guide](https://dortania.github.io/OpenCore-Install-Guide/) and boot into the Catalina installer.  I did miss a step on the "boot-args" for the GPU I'm using and once that was sorted I finished the "startup" and had a running system.

Feel free to grab anything that will help!

## Hardware:

| **MB:**      | [MSI MEG Unify](https://www.msi.com/Motherboard/MEG-X570-UNIFY/Specification) |
| :----------- | :----------------------------------------------------------- |
| **CPU:**     | [AMD Ryzen 3700x](https://www.amd.com/en/products/cpu/amd-ryzen-7-3700x) |
| **RAM:**     | [64GB(4x16GB) 3200mhz DDR4 Leven Sinba PC25600](https://www.amazon.com/gp/product/B08M66XV22/ref=ppx_yo_dt_b_asin_title_o09_s00?ie=UTF8&psc=1) |
| **GPU:**     | [(currently)PC Partner - Radeon 8760 2GB](https://evertek.com/Product/H88-3E243-101A8-CO-PB-R) |
| **Storage:** | [Samsung Evo 970 2TB Nvme](https://www.amazon.com/Samsung-970-EVO-Plus-MZ-V7S2T0B/dp/B07MFZXR1B) |
| **Wifi:**    | Onboard Intel wifi 6 AX200                                   |
| **LAN:**     | Onboard Intel Realtek® RTL8125 2.5 Gbps                      |
| **Sound:**   | Onboard Realtek® ALC1220                                     |

## **What's working/not working**:

**OSX Catalina 10.15.7**
Opencore 6.4

**Sound**

"working" ok except for the lack of mic support on the kext for the ALC1220.

**Wifi**

Working with [Heliport](https://github.com/OpenIntelWireless/HeliPort) and [itlwm](https://github.com/OpenIntelWireless/itlwm) for the AX200.

**LAN**

I've used the ["Lucy" 8125 kext](https://github.com/Mieze/LucyRTL8125Ethernet). I have not yet run a cable over to where my computer is being used for the winter. Currently I'm using wifi.  I did test the lan card using some "network over power" adapters I have but since I have shielded wired gigabit back-haul to my Ubiquity wifi APs, the wifi is faster than the power adapters. (old house with lots of crazy wiring slowing it down)

**Bluetooth**

Bluetooth on the AX200 is working fine for output ( no mic ) to my various headphones etc.

**iSight camera**

The  camera on my old faithful 27" 2K "Cinema Display" (mini-display with USB not thunderbolt) is not functioning.  It works after boot the 1st time I start FaceTime but then gets disabled somehow. I'm just getting a cheapo $35 webcam from Amazon for my conference calls. I tested one I bought for my kid and it's working fine with all my conf apps.  Speakers and mic work on that but the mic is pretty bad so I hooked up a decent extra USB mic I had around and that works great.

Overall I'm pretty happy with the build.  The machine seems to run nice and fast.
