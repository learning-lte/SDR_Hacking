# SDR_Hacking
In this repository I will explain the various programs and scripts that I used to learnd and do different cool things with my HackRF one. I also include programs that have already been made and/or compiled and provide my own compilation and settings for Windows 10.

So what is **SDR** or **Software-Defined Radio**, SDR is a radio communication system where components that have been traditionally implemented in hardware (e.g. mixers, filters, amplifiers, modulators/demodulators, etc.) are instead implemented by means of software on a personal computer.

There are quite a few affordable SDR to buy, the most famous ones include [RTL SDR](https://www.rtl-sdr.com/buy-rtl-sdr-dvb-t-dongles/), [HackRF One](https://greatscottgadgets.com/hackrf/) (This is an Open Source SDR and the one I bought from [Banggood](https://es.banggood.com/HackRF-One-1MHz-6GHz-Radio-Platform-Development-Board-Software-Defined-RTL-SDR-Demoboard-Kit-Dongle-Receiver-Ham-Radio-p-1552853.html?rmmds=search), a lot cheaper than the original one), [NooElec](https://www.nooelec.com/store/sdr/sdr-receivers/nesdr-smartee-xtr.html), etc.

## **SDR specifications**

Each SDR has different specifications, some of them are:

- **Bandwidth**: How much of the Electromagnetic spectrum you are able to receive, most of them go from 27Mhz all the way to 1.7Ghz. I bought the HackRF One for its huge bandwidth that ranges from 1MHz all the way to 6GHz. Remember to use an antenna tuned for the specific frequency you are working with, as an antenna tuned for 433MHz won't do a good job of listening to WiFi signals (2.4GHz).

- **Receiving and/or transmitting**: Most of the SDRs I listed don't have the capacity of outputting any signals. The HackRF One has that capability, its output power ranges from 1mW to 30mW depending on the frequency. So don't expect to output anything beyond a couple of meters.

## **SDR Software**

Once you have your SDR on your hands it's time to decide what to do with it. Do you just want to listen to FM radio with it? Do you want to listen to amateur ham radio? Do you want to see the electromagnetic spectrum produced by the different devices around your house? Do you want to receive live images from satellites? Do you want to hack every garage door? Do you want to spoof GPS signals? Do you want to see other people's screen by picking up their HDMI noise?

The possibilities are endless!, even though each application uses a different program, you will spend most of your time in only a couple of them. Let's go through some of my favourite programs and what each one of them does. Again I mostly use Windows 10, not very familiar with Linux, I will provide its Linux or macOS counterpart whenever I can.

- **[SDR#](https://airspy.com/download/)**: Free, but not Open Source, the most used SDR software in Windows, it is an easy and lightweight program that allows you to visualize the frequency spectrum and demodulate the signal you are looking at. Since it is so well known, lots and lots of [plugins](https://www.rtl-sdr.com/sdrsharp-plugins/) are available for it. You can demodulate PAL, NTSC, DSD, Tetra...

    ![SDR#](https://github.com/Hanqaqa/SDR_Hacking/blob/master/media/SDRSharp.PNG)


    Its Linux and macOS counterpart is called [GQRX](https://gqrx.dk/), it is Open Source and easy  to use, although it doesn't have as many plugins as SDR#.

- **[Universal Radio Hacker](https://github.com/jopohl/urh)**: An Open Source and easy to use signal analyzer. I learnt more using this program for a few hours than with several years of signal analysis in my university. With this program you can easily demodulate and see the info that is travelling through the air of whatever device you want to learn about, keyfobs, FM Radio Stations, weather stations... Although one thing is seeing the ones and zeroes travelling through the air and a very different thing is reverse engineering how that series of ones and zeroes was produced. Also available on Linux and macOS.

- **[GNU Radio](https://www.gnuradio.org/)**: The father of all the SDR applications. It is an Open Source development toolkit that provides signal processing blocks to implement software-defined radios and signal-processing systems. Requires a very good knowledge of all the modulation and demodulation techniques as well as general knowledge of flowgraph programming. There is a big number of premade modules. Available for all platforms.

## **SDR in the law**

