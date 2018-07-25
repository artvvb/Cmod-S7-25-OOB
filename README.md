Cmod S7-25 Out-of-Box Demo
==============

Introduction
--------------
This project is a simple Verilog demo using the Cmod S7-25's LEDs, RGB LED, buttons, and USB-UART bridge. When programmed onto a board, the RGB LED will cycle from Blue to Green to Red to Black. The other LEDs will light up in sequence. Whenever one of the two buttons is pressed, "Button # Pressed!" is sent to a connected PC using the USB-UART bridge.

Using This Demo
--------------
Requirements:
* [Cmod S7-25](https://store.digilentinc.com/cmod-s7-breadboardable-spartan-7-fpga-module/)
* [Vivado 2018.2 Installation](https://reference.digilentinc.com/vivado/installing-vivado/start)
* [Tera Term Installation](https://ttssh2.osdn.jp/index.html.en) or other serial terminal application
* MicroUSB Cable

Release Usage:

1. Download and extract the release ZIP archive.
2. Open project in Vivado 2018.2 (\<archive extracted location\>/vivado_proj/Cmod-S7-25-OOB.xpr).
3. In the *Flow Navigator* panel to the left of the Vivado window, click "Open Hardware Manager".
4. Plug a Cmod S7-25 into the computer running Vivado using a MicroUSB cable.
5. Open a serial terminal application (such as TeraTerm FIXME LINK) and connect it to the Cmod S7's serial port, using a baud rate of 9600.
6. Click "Open target" in the green bar at the top of the window. Select "Auto connect" from the drop down menu.
7. Click "Program device" in the green bar at the top of the window. In the "Program Device" wizard, enter "\<archive extracted location\>vivado_proj/Cmod-S7-25-OOB.runs/impl_1/top.bit" into the "Bitstream file" field. Then click *Program*.
8. The demo will now be programmed onto the Cmod S7. Refer to the *Introduction* section of this README for more information on how to use it. The demo can be modified through the Vivado *Proejct Manager*.

<!--- FIXME Tera Term ... --->

For more information on how this project is version controlled refer to the [Digilent Vivado Scripts Repository](https://github.com/artvvb/digilent-vivado-scripts)