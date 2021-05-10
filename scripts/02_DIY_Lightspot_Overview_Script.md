# 02 DIY Lightspot Overview Script

1. Get a working Device
    - This step varies wildly and depends on your skill level
    - In theory anything that has a lora concentrator, can run linux, and has an architecture supported by the rust compiler is capable of being a diy packet forwarder
    - More realistically for anyone who isn't a savant embedded developer, you will need a device with a lora concentrator capable of running linux, the things network gateway and gateway rs. The most restrictive point is gateway-rs, as it
    requires both linux and a chip architecture that the rust compile can target.
    - At the basic end of the spectrum is the dragino, which comes built, with linux installed and the things network gateay installed.
    - At the intermediate level we have the DIY rak units. These are typically sold as a kit, and includes a RAK enclosure, RAK raspberry pi lorawan shield, a lora antenna, a GPS antenna and a raspberri pi. These units require a bit more work, not only do you have to build them, you have to flash them with a vendor supplied custom raspbian image. The custom raspbian image comes with almost all the applications you need installed. The only application you'll need to install yourself is gateway-rs.
    - At the advanced level you probably don't need me to tell you what to do. However, from my investigations the limit factor is gateway-rs which has a dependency on linux, and is written in rust so can only be compiled for architectures that rust currently supports. It's more than likely possible to re-write the things network packet forwarder and gateway-rs for a more minimal device.

2. Setup Device
    - These next steps will vary considerably depending what device you are using
    - The first step is to connect to the internet, depending on your unit you may or may not need to set a static ip
    - The next step is to set up the packet forwarder, change the ports to forward to 1680
    - Next download gateway-rs to your computer and install it
    - Reboot the raspberry pi
    - Check that helium_gateway service is running and is printing logs
    