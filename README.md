
A vacuum fluorescent display (VFD) is a [display device]once commonly used on consumer electronics equipment such as [video cassette recorders], [car radios], and [microwave ovens].

A VFD operates on the principle of [cathodoluminescence], roughly similar to a [cathode ray tube], but operating at much lower voltages. Each tube in a VFD has a [phosphor]-coated carbon [anode] that is bombarded by electrons emitted from the [cathode filament]. In fact, each tube in a VFD is a [triode] vacuum tube because it also has a mesh control grid

Unlike [liquid crystal displays], a VFD emits very bright light with high contrast and can support display elements of various colors. Standard illumination figures for VFDs are around 640 [cd/m2] with high-brightness VFDs operating at 4,000 cd/m2, and experimental units as high as 35,000 cd/m2 depending on the drive voltage and its timing. The choice of color (which determines the nature of the phosphor) and display brightness significantly affect the lifetime of the tubes, which can range from as low as 1,500 hours for a vivid red VFD to 30,000 hours for the more common green ones.) [Cadmium] was commonly used in the phosphors of VFDs in the past, but the current [RoHS]-compliant VFDs have eliminated this metal from their construction, using instead phosphors consisting of a matrix of alkaline earth and very small amounts of group III metals, doped with very small amounts of rare earth metals.

VFDs can display [seven-segment] numerals, multi-segment alpha-numeric characters or can be made in a dot-matrix to display different alphanumeric characters and symbols. In practice, there is little limit to the shape of the image that can be displayed: it depends solely on the shape of phosphor on the anode(s).

The first VFD was the single indication DM160 by Philips in 1959. The first multi-segment VFD was a 1967 Japanese single-digit, seven-segment device. The displays became common on calculators and other consumer electronics devices. In the late 1980s hundreds of millions of units were made yearly.
Design

Macro image of a VFD digit with 3 horizontal tungsten wires and control grid
The device consists of a hot cathode (filaments), grids and anodes (phosphor) encased in a glass envelope under a high vacuum condition. The cathode is made up of fine tungsten wires, coated by alkaline earth metal oxides (barium,[2] strontium and calcium oxides[8][9]), which emit electrons when heated to 650 ??C[2] by an electric current. These electrons are controlled and diffused by the grids (made using Photochemical machining), which are made up of thin (50 micron thick) stainless steel.[2] If electrons impinge on the phosphor-coated anode plates, they fluoresce, emitting light. Unlike the orange-glowing cathodes of traditional vacuum tubes, VFD cathodes are efficient emitters at much lower temperatures, and are therefore essentially invisible.[10] The anode consists of a glass plate with electrically conductive traces (each trace is connected to a single indicator segment), which is coated with an insulator, which is then partially etched to create holes which are then filled with a conductor like graphite, which in turn is coated with phosphor. This transfers energy from the trace to the segment. The shape of the phosphor will determine the shape of the VFD's segments. The most widely used phosphor is Zinc-doped copper-activated Zinc oxide,[2] which generates light at a peak wavelength of 505 nm.

The cathode wire to which the oxides are applied is made of tungsten or ruthenium-tungsten alloy. The oxides in the cathodes are not stable in air, so they are applied to the cathode as carbonates, the cathodes are assembled into the VFD, and the cathodes are heated by passing a current through them while inside the vacuum of the VFD to convert the carbonates into oxides.[2][9]

The principle of operation is identical to that of a vacuum tube triode. Electrons can only reach (and "illuminate") a given plate element if both the grid and the plate are at a positive potential with respect to the cathode.[11] This allows the displays to be organized as multiplexed displays where the multiple grids and plates form a matrix, minimizing the number of signal pins required. In the example of the VCR display shown to the right, the grids are arranged so that only one digit is illuminated at a time. All of the similar plates in all of the digits (for example, all of the lower-left plates in all of the digits) are connected in parallel. One by one, the microprocessor driving the display enables a digit by placing a positive voltage on that digit's grid and then placing a positive voltage on the appropriate plates. Electrons flow through that digit's grid and strike those plates that are at a positive potential. The microprocessor cycles through illuminating the digits in this way at a rate high enough to create the illusion of all digits glowing at once via persistence of vision.

The extra indicators (in our example, "VCR", "Hi-Fi", "STEREO", "SAP", etc.) are arranged as if they were segments of an additional digit or two or extra segments of existing digits and are scanned using the same multiplexed strategy as the real digits. Some of these extra indicators may use a phosphor that emits a different color of light, for example, orange.

The light emitted by most VFDs contains many colors and can often be filtered to enhance the color saturation providing a deep green or deep blue, depending on the whims of the product's designers. Phosphors used in VFDs are different from those in cathode-ray displays since they must emit acceptable brightness with only around 50 volts of electron energy, compared to several thousand volts in a CRT. The insulating layer in a VFD is normally black, however it can be removed to allow the display to be transparent. AMVFD displays that incorporate a driver IC are available for applications that require high image brightness and an increased number of pixels. Phosphors of different colors can be stacked on top of each other for achieving gradations and various color combinations. Hybrid VFDs include both fixed display segments and a graphic VFD in the same unit. VFDs may have display segments, grids and related circuitry on their front and rear plass panels, using a central cathode for both panels, allowing for increased segment density. The segments can also be placed exclusively on the front instead of on the back, improving viewing angles and brightness.
Besides brightness, VFDs have the advantages of being rugged, inexpensive, and easily configured to display a wide variety of customized messages, and unlike LCDs, VFDs are not limited by the response time of rearranging liquid crystals and are thus able to function normally in cold, even sub-zero, temperatures, making them ideal for outdoor devices in cold climates. Early on, the main disadvantage of such displays was their use of significantly more power (0.2 watts) than a simple LCD. This was considered a significant drawback for battery-operated equipment like calculators, so VFDs ended up being used mainly in equipment powered by an AC supply or heavy-duty rechargeable batteries.
this display has a 14 characters, consist of 5*7 dot matrix in the first row, and icon's to display for example WIFI and Bluetooth and 14 segments 9 digits and 7 segments 2 digits in the second row.

.I did use two SN75518 Vacuum fluorescent display drivers, to control the dots and segments and icons and grids in the display. it has 60-v output voltage swing capability, and 25-mA output source current capability, and high-speed serially shifted data input, latch on all driver outputs. Each device consists of a 32-bit shift register, 32

latches, and 32 output AND gates. Serial data is

entered into the shift register on the low-to-high

transition of CLOCK. While LATCH ENABLE is

high, parallel data is transferred to the output

buffers through a 32-bit latch. Data present in the

latch during the high-to-low transition of LATCH

ENABLE is latched. When STROBE is low, all Q

outputs are enabled. When STROBE is high, all Q

outputs are low.

I did connect the first dot to the firs Q1 in the SN75518 Vacuum fluorescent display drivers and the second dot to the Q2 and so on. to the last Q32,the last 3 dots connected to the second SN75518.

the firs SN75518 to control the 32 dots in the first row, and the icons and the 14 segments and 7 segments in the second row.

the second SN75518 to control grids, this display has 20 grids for the first and the second row.

and I did use the last 5 Q of the second SN75518 to control the rest of last 3 dots in the first row.

I did cascade the first SN75518 to the second SN75518 throw serial out

and I did use Arduino seeeduino Xiao to control the two SN75518 Vacuum fluorescent display drivers by utilize SPI to send data at speed of 1000000 MHZ to the display ,and I utilize I2C to receive data from any other Arduino board like uno,nano,mega.by using library I did belt I called VFDI2CMster to send data over I2C, which is compatible with other Arduino boards.

Serial peripheral interface (SPI) is one of the most widely used interfaces between microcontroller and peripheral ICs such as sensors, ADCs, DACs, shift registers, SRAM, and others.

SPI is a synchronous, full duplex main-subnode-based interface. The data from the main or the subnode is synchronized on the rising or falling clock edge. Both main and subnode can transmit data at the same time. The SPI interface can be either 3-wire or 4-wire. This article focuses on the popular 4-wire SPI interface.

.In my case I use only MOSI and SCK only. to connect to data and clock in the SN75518.

SCK go to the first and second SN75518 CLOCK pin #21.

MOSI go to the first SN75518 DATA pin #39, and SERIAL OUT from the first SN75518 to second SN75518, that called cascade.

Serial data output from the shift register may be

used to cascade additional devices. This output is

not affected by LATCH ENABLE or STROBE.

5-V for SN75518 and Arduino seeeduino Xiao.

5-V for [cathode filament].

28-V for dots and segments and grids.
first I did create array of type byte consist of 4 element called shiftRegisterBytes[4]; to carry data for all dots and segments and icons in the display by using return type method that return array type of byte. in the DisplayData.h code

second star sending grid data and then dots or segments data over SPI SPI.beginTransaction(SPISettings(1000000,LSBFIRST,SPI_MODE3));because of the SN75518 , the serial data is entered into the shift register on low-to-high

I did utilize I2C to receive data over I2C from any Arduino board. by using library I did belt I called VFDI2CMster to send data over I2C

I did program ever thing using visual code IDE and platform IO.
