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
* Cleaned up code formatting, indentation, etc.
* Lowered volume from 1750 to 450.
* Disabled flickering effect on: Sabertrio, Dark Edition, The Dark, Vengeance, Temple Guardian, The Tragedy, Smooth Jedi, Smooth Grey, Smooth Fuzz.

## [props/s3button_config.h](props/s3button_config.h)
* (none yet)

# References and Notes

## Example blade configuration

Tip: Don't like the color of the activation switch your saber shipped with? Set the 4th "blade" in the
below config to `StylePtr<Black>()` and it'll turn off the LED.

```c

Preset blade[] = {
	{
		// Soundfont Directory Name
		"0-NO_BLADE",

		// Leave blank - unused?
		"",

		// Primary Blade Style
		StylePtr<Black>(),

		// Cross-guard blade styles. Probably ignored unless you have a Krosgaard saber.
		StylePtr<Black>(),
		StylePtr<Black>(),

		// Activation Switch
		StylePtr<WHITE>(),

		// Blade preset profile name - not sure how this is used, but should probably be unique.
		"ProfileName"
	}
}

```


## Disable Main Button LED

Did you get one of Sabertrio's RTS (ready-to-ship) sabers, but don't like the activation switch
LED color that it shipped with? Or did you customize a saber but then regret the choice of LED?

In Sabertrio's configuration, the power button's LED is wired in as the 4th "blade" on the
Proffieboard. You can disable the LED by switching the 4th blade style in the `blades[]` array
from `StylePtr<WHITE>()` to `StylePtr<Black>()`.

You'll have to do this per blade style. You can, of course, also choose to leave it on with
some blade styles and off with others. (That's what I did - I left it on for the blade styles
that happen to match the LED color, and off for the others!)


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
