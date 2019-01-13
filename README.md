# RetroPie-BeebEm

This is a fork of https://github.com/zerojay/RetroPie-Extra-unstable
It's only purpose is to make installing BeebEm to RetroPie easier.
For that reason everything not related to BeebEm has been removed.

Changes
1) A bug in the original set-up script, that failed to specifiy the appropriate file extentions for BeebEm, has been fixed.
2) The installer now targets a version of BeebEm forked from https://github.com/roksoft/beebem-retropie which includes the ability to re-map BeebEm keys to those used by the Picade joystick and buttons (or in fact any other controller).
3) An example of a key remapping file is provided, see here https://retropie.org.uk/forum/topic/2261/beebem-and-fun-arcade-control-modifications for details.

## Installation.

If you have BeebEm already installed by other means (e.g. via zerojay's Extra-unstable repo) then you will *probably* need to uninstall it via the RetroPie setup menu first (make any backups you think you may need!!)

1) Plug a USB keyboard into you RetroPi/Picade machine.

2) When in EmulationStation (i.e. not running a game), hit F4 on the keyboard to bring up a console.

3) Clone this repoo:
```
git clone https://github.com/GandalfUK/RetroPie-BeebEm.git
```

4) Run the install script from within the repo directory (you may have to make the script executable):
```
cd RetroPie-BeebEm
chmod a+x install.sh
./install.sh
```
5) Exit the console (type `exit`) and go to the RetroPie setup menu. Select the Manage Packages option and choose the Experimantal packages. You should now see BeebEm in the list. Select BeebEm and install it.

That's it! Put your game-files/disk-images in roms/beebem/ as you would for any other system. If you want to use the key re-mapping features, copy you map file in here too (there is an example map-file for snapper provided in the `BeebEm-maps` dir. Note that the name of the map file(s) must match the name of the game/disk-image file(s). 

