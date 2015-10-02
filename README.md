# mcbmini
Automatically exported from code.google.com/p/mcbmini

Overview

MCBMini is a complete and open-source motor control solution. It includes the hardware design files for PCBs, firmware, partslists and suppliers, firmware for micro controllers and java host software.
Table of contents

    Overview
    Features
    Images
    Licenses
    Documentation
    How to get them

		

Features

Each board has two motor control channels, each spec is "per channel" but eacg board can also be run in "joint" mode where two channels can be used to control one (beefy) motor.

    Separate logic and motor power sources (can be use single power source with jumper setting)
    Logic power voltage range: 6-24V
    Motor power voltage range: 5.5-24V
    Maximum channel output current: 30A (max current of bridge, heat considerations need to be made)
    PWM frequencies of 20kHz (inaudible)
    Velocity and position PID closed-loop control
        Maximum velocity and acceleration parameters 
    Position feedback: Quadrature encoder or potentiometer (or both)
    Current sensing
    Communication to MCBCom board supports:
        TTL level serial (RX/TX)
        USB bia USB-mini connector (using FTDI technology)
        Bluetooth via socket for the SparkFun BlueSMIRF board 
    Electrical protection:
        Output short to GND or Power shutdown (with software notification)
        Thermal shutdown (with software notification)
        Reverse battery protection (for motor power) 
    2 extra pins per board which can each be configured to:
        Read an external analog voltage
        Monitor Logic/Motor batteries (each has dedicated extra pin)
        Read switch state (possibly a limit switch) and notify software of event
        Control servo motor (create pulse signal needed by a servo) 
        
  Licenses

This project contains three different kinds of licenses:

    MCBMiniServer (the java host software): LGPLv2
    PCB designs (both for motor controllers and communication board): CC w/Attribution
    Motor control firmware: GPLv2 

Documentation

Manuals can be found in the Downloads section of this site 
