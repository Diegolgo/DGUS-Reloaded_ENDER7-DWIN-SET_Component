
Working on Klipper v0.13.0-642-g77d5d942  (May 07 2026)

This is very simple if you have previous version of lcd working on klipper, so go to step 1. if you dont, stay here in step 0 (cr6 and ender7 are the same screen, just rotated)
Step 0: research:
so, is too much to explain everything, but the simple steps:
flash the lcd with desuu info here: 
https://github.com/Desuuuu/DGUS-reloaded
and here
https://github.com/capekoviroboti/creality-dwin-lcd-customizer
you can edit, rotate, and do a lot , but i only need to "see" the progress, temp, or maybe sometime use touchscreen (with mainsail is all on web browser)
a very good example is here:
https://github.com/fryc88/klipper-sv06plus-screen

Step 1 (skip if you want to use the firmware precompiled):
use the folder make_menuconfig_Extensions, to put files inside klipper and make the "new" version of firmware to Ender 7.
credits to DGUS-Reloaded_for_CR6-Klipper_Component-2.0.0 link https://github.com/Thinkersbluff/DGUS-Reloaded_for_CR6-Klipper_Component
enter to kiauh (or make yourself in linux)
compile the firmware version normaly (you gonna now have the DGU option in make menu)
that's it.
put the firmware.bin in a sd card, plugin in the Ender 7 printer. turn off , and turn on. just a couple of second...

Step 2
in klipper via Filezila or something like that, you need to put the folder: t5uid1 inside klippy/extras/ THIS HAVE TO BE THIS EXACT FOLDER, newer version broke the comunication with the printer, some of the .py files have errors and so on... (this is a previous version of DGU)

Step 3 
restart printer and MCU
that's all.
done

now you have latest version of klipper, and lcd with touchscreen with commands working (movements, heating, PID, config, progress, etc etc)

note: if you gonna use my printer.cfg and other, notice that  need to call some of others .cfg from there , like cr6.cfg etc.
very important to put DGU_START_PRINT inside START_PRINT wherever you have that...







## Credits
| Material                                                                       | Author                                                    | Modified | License                                                               |
|:------------------------------------------------------------------------------:|:---------------------------------------------------------:|:--------:|:---------------------------------------------------------------------:|
| [DGUS-RELOADED DWIN UI](https://github.com/Desuuuu/DGUS-reloaded-Klipper)      | [Desuuuu](https://github.com/Desuuuu)                     | Yes      | [GPLv3](http://www.gnu.org/licenses/gpl-3.0.html)   
| [Klipper logo](https://github.com/KevinOConnor/klipper)                        | [KevinOConnor](https://github.com/KevinOConnor)           | Yes      | [GPLv3](http://www.gnu.org/licenses/gpl-3.0.html)                     |
| [Feather icons](https://feathericons.com/)                                     | [Cole Bemis](https://twitter.com/colebemis)               | Yes      | [MIT](https://github.com/feathericons/feather/blob/master/LICENSE)    |
| [3D Printing Line icons](https://www.iconfinder.com/iconsets/3d-printing-line) | [Sam Baines](https://www.iconfinder.com/conceptbaines)    | Yes      | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/legalcode)    |
| [Fan icon](https://thenounproject.com/term/fan/1153915/)                       | [Atif Arshad](https://thenounproject.com/atifarshad/)     | Yes      | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |
| [Snow icon](https://thenounproject.com/term/snow/1959859/)                     | [Shashank Singh](https://thenounproject.com/rshashank19/) | Yes      | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |
| [Electric Motor icon](https://thenounproject.com/term/electric-motor/2734486/) | [Verry](https://thenounproject.com/verry.dsign.creative)  | Yes      | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |
| [Probe icon](https://thenounproject.com/term/probe/1841345/)                   | [Mohamed Mbarki](https://thenounproject.com/mb.icons)     | Yes      | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |
| [Wheel icon](https://thenounproject.com/term/wheel/92430/)                     | [Deivid Sáenz](https://thenounproject.com/deivid.saenz)   | Yes      | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |
| [Ruler icon](https://thenounproject.com/term/ruler/1738925/)                   | [Three Six Five](https://thenounproject.com/365)          | -        | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |
| [Wrench icon](https://www.flaticon.com/free-icons/preferences)                | [Freepik - Flaticon](https://www.flaticon.com)            | Yes      | [Free-Use](https://www.freepikcompany.com/legal?&_ga=2.208290896.334573684.1672634783-793280358.1672634783&_gl=1*bcixj4*fp_ga*NzkzMjgwMzU4LjE2NzI2MzQ3ODM.*fp_ga_1ZY8468CQB*MTY3MjYzNDc4My4xLjEuMTY3MjYzNDgzMC4xMy4wLjA.*test_ga*NzkzMjgwMzU4LjE2NzI2MzQ3ODM.*test_ga_523JXC6VL7*MTY3MjYzNDc4My4xLjEuMTY3MjYzNDgzMS4xMi4wLjA.#nav-flaticon-agreement) |
Emergency Stop icon copied from [KlipperScreen](https://github.com/jordanruthe/KlipperScreen) | [Jordan Ruthe](https://github.com/jordanruthe)  | Yes        | [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/us/legalcode) |

## License
[GPLv3](http://www.gnu.org/licenses/gpl-3.0.html)
