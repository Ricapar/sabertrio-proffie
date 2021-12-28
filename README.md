# Sabertrio Lightsaber - ProffieOS Configuration

This repository only includes a copy of the GPL'd ProffieOS code, including Sabertrio's modifications to the blade
profiles and button configurations. It does not include any soundfonts.

The code as I got it off of the saber's SD card can be found on the [sabertrio-backup](https://github.com/Ricapar/sabertrio-proffie/tree/sabertrio-backup)
branch of this repo. My own changes can be found on the master branch. Feel free to do a diff between the two to see what I've changed. I'll try to keep
key changes listed below.

Additonal information here is also for my own reference.

# Key Files

I suspect that outside of these files, the rest of ProffieOS is unchanged. As such this is where I'm focusing most of my attention
on cleanup and tweaking.

* [config/s3config.h](config/s3config.h)
* [props/s3button_config.h](props/s3button_config.h)

# Changelog

## [config/s3config.h](config/s3config.h)
* Lowered volume from 1750 to 450.
* Disabled flickering effect on: Sabertrio, Dark Edition, The Dark, Vengeance, Temple Guardian, The Tragedy, Smooth Jedi, Smooth Grey, Smooth Fuzz.

## [props/s3button_config.h](props/s3button_config.h)
* (none yet)

# References and Notes

##  Blade Settings

* 1-SABERTRIO Fully Responsive RandomFlicker Blade Style ( DodgerBlue ) (animated)
* 2-DARK_EDITION Fully Responsive RandomFlicker Blade Style ( Red ) (animated)
* 3-THE_LIGHT Fully Responsive RandomFlicker Blade Style ( DeepSkyBlue ) (original)
* 4-THE_BALANCE Fully Responsive RandomFlicker Blade Style ( Green ) (prequel)
* 5-THE_DARK Fully Responsive RandomFlicker Blade Style ( Red ) (original)
* 6-VENGEANCE Fully Responsive RandomFlicker Blade Style ( Red ) (animated)
* 7-KROSSGUARD Fully Responsive Kylo Ren Unstable Neopixel Lightsaber (Unstable Swing) Styles ( Red ) (sequel)
* 8-SNIPPETS Fully Responsive AudioFlicker Canon Jedi/Sith Neopixel Lightsaber Styles ( Silver ) (animated)
* 9-MENACE Fully Responsive RandomFlicker Blade Style ( Red ) (prequel)
* 10-TEMPLE_GUARDIAN Fully Responsive RandomFlicker Blade Style ( Gold ) (animated)
* 11-SHOCK_BATON Shock Baton Neopixel Lightsaber Style ( Shock Baton ) (sequel) (polar spark,center in)
* 12-THE_TRAGEDY Fully Responsive AudioFlicker Canon Jedi/Sith Neopixel Lightsaber Styles ( Red ) (prequel)
* 13-TEENY_SF Fully Responsive RandomFlicker Blade Style ( Cyan ) (prequel)
* 14-SMOOTH_JEDI Fully Responsive RandomFlicker Blade Style ( Blue ) (original)
* 15-SMOOTH_GREY Fully Responsive AudioFlicker Canon Jedi/Sith Neopixel Lightsaber Styles ( Amber/Gold ) (sequel)
* 16-SMOOTH_FUZZ Fully Responsive RandomFlicker Blade Style ( Purple ) (prequel)
* 17-ROGUE_COMMANDER Fully Responsive "Power Surge" Unstable Neopixel Lightsaber Style ( Red ) (original)
* 18-TYTHONIAN_CYRSTAL Fully Responsive RandomFlicker Blade Style ( Green ) (original)
