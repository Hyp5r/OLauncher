# OLauncher

## Usage

### Command Line

`OLauncher.exe "<path to Origin>" "<Origin.exe>" "<path to Origin Game>" "<Game.exe>" "<RunAsAdmin>" "<CloseOriginAfter>"`

* `<path to Origin>` is the install directory where Origin resides, usually `C:\Program Files (x86)\Origin`
* `<Origin.exe>` is usually `Origin.exe`. This won't change unless EA changes Origin's executable name.
* `<path to Origin Game>` is the install directory where the game you want to run resides.
  * As an example, let's say Mass Effect Andromeda, which is installed to `D:\Games\Origin Games\Mass Effect Andromeda`
* `<Game.exe>` is the game executable.
  * In Mass Effect Andromeda's case, it would be `MassEffectAndromeda.exe`.
* `<RunAsAdmin>` is either `0` or `1`.
  * `0` means that OLauncher will not attempt to run as an administrator.
  * `1` means that OLauncher will attempt to run as an administrator.
  * If you run OLauncher as admin, OLauncher will automatically overwrite any saved INI in the same directory. This is because OLauncher does not read the command line arguments again after running OLauncher, so it will store all values before restarting. If you like to run with INI files rather than launching from the command line, it's recommended to make multiple copies of OLauncher in different directories.
* `<CloseOriginAfter>` is either `0` or `1`.
  * `0` means keep Origin open after closing the game.
  * `1` means close Origin after closing the game.

#### Examples

* Launching Mass Effect Andromeda, do not run as an admin and close Origin when done:

  `OLauncher.exe "C:\Program Files (x86)\Origin" "Origin.exe" "D:\Games\Origin Games\Mass Effect Andromeda" "MassEffectAndromeda.exe" 0 1`

* Launching the original Mass Effect, run as an admin and close Origin when done:

  `OLauncher.exe "C:\Program Files (x86)\Origin" "Origin.exe" "D:\Games\Origin Games\Mass Effect\Binaries" "MassEffect.exe" 1 1`

### INI File

OLauncher supports launching through an INI file as well. If you run `OLauncher.exe` without any command line arguments, OLauncher will generate an INI in the directory where it was run. From there, you can fill out the game details and save the file. Running `OLauncher.exe` again with the INI beside it will launch whatever is found in the INI.

## About the Script

OLauncher is a script that allows you to launch Origin games from within
the Steam client.  Launching games through this script is automated,
from automatically starting Origin to launching the game that is listed
within the OLauncher.ini file.  Once the game is shutdown, the script
will ask if you would like to keep Origin running or shut it down as
well.

Running Origin games through this script should allow the Steam overlay
to work, though not guaranteed.

## Disclaimer

By using this script in any way, you agree to the following disclaimer:

I am, in no way shape or form, related to or involved in Origin, EA,
Electronic Arts, or any similar entity. Origin is Copyright © 2017
Electronic Arts Inc.

I am not responsible for your use of this script. I am also not
responsible if this script works as intended, blows up your computer,
eats your lunch, fails to do what you expect, or becomes sentient. I
am not obligated in any way to support the use of this script, or give
support to you for this script.

## Credits

The icon used in the compiled EXE was created by **Pixel Buddha** and can be found by going to https://www.flaticon.com/free-icon/gamepad_214304.
