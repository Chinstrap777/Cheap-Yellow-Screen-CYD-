# Instructions for Cheap Yellow Display (CYD) using Klipper 3D printers

## Teaching Tech Video with instructions
https://www.youtube.com/watch?v=R3o0MGYW1ZU&list=LL&index=9 

# CYD-Klipper
An implementation of a wireless Klipper status display on an ESP32 + screen. Uses Moonraker to fetch data.

A simple and cheap solution to use a dedicated screen with Klipper, a 3d printing Firmware.

![showcase_image](readme/PXL_20231113_171629383.jpg)

### Required hardware

A ESP32-2432S028R is required to run this project. You can find out where to buy these on the ["ESP32 Cheap Yellow Display"](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display#where-to-buy) repository.

### Features
- View printer status
- View print progress
- Start a print
- Move the printer
- Manage temperature
- Extrude/Retract filament
- Execute predefined gcode macros

### Install

[There is a web-based installer available. This is only supported on Chrome, Edge or Opera, and only on Desktop.](https://suchmememanyskill.github.io/CYD-Klipper/)

On initial install, all data should be wiped. On updates, data should be able to be kept without issues.

There are no 'over the air' updates. Each update has to be applied manually.

1. Connect CYD to PC with micro USB cord (must have data).
   or
   Connect using bluetooth after finding in Terminal (MAC).
2. Go to above site for installer.

3. Select which COM port you want to use to connect to the CYD (I use USB).
4. Click "Install CYD Klipper".
5. Enable "Erase Device" and click "Next" (Only on initial setup, you won't erase after that).
6. Click "Boot" button immediately after the previous step.
7. Calibrate the screen with the stylus when it has completed installing
8. Input wifi SSID and Password
9. Input Mainsail/Fluid/Pi IP address (192.168.x.x) and leave in Port 80
10. For any macros you want to run from the CYD, input the following in the "description" field like this:
    description: CYD_SCREEN_MACRO

### Screenshots
(Quite literally shots of the screen. I'm sorry)

-|- 
:-:|:-:
![1](readme/PXL_20231113_142717308.jpg)|![2](readme/PXL_20231113_171701876.jpg)
![3](readme/PXL_20231113_171715809.jpg)|![4](readme/PXL_20231113_171724404.jpg)
![5](readme/PXL_20231113_171751745.jpg)|![6](readme/PXL_20231113_171809315.jpg)


### Credits
- [xtouch](https://github.com/xperiments-in/xtouch)
- [ESP32-Cheap-Yellow-Display](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display)
