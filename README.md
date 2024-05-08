# AkiraFlex
AkiraFlex is an N64 RDRAM termination flex PCB, designed to be a low-profile replacement for the stock expansion port + trimmed jumper pak combo commonly used in existing N64 portables. It was inspired by the ["Akira Method"](https://bitbuilt.net/forums/index.php?threads/lockdown-64.4175/post-46301) of digging up the expansion port pads and deadbugging the RDRAM termination circuit.

<img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/layout.PNG" width=500>\
<img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/render-front.PNG" width=500> <img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/render-back.PNG" width=500>

## Installation
Components for the flex can either be pulled from an original N64 jumper / expansion pak, or can be bought brand new. All RAs are 1206-sized 51 Ohm, all caps are 0603-sized 1uF.

This flex was originally designed around a NUS-CPU-03 board, which has test points on the RDRAM traces between the RAM and the expansion port. If you are using this on a non-Rev 3 board (such as the Rev 4 board I installed in on here), you will need to scratch the traces as shown. Additionally, the VREF and VTERM vias must be scratched / tinned. Though apparently not necessary according to some testing Cy (of the BitBuilt Forums) has done, it is best practice to dig up the existing expansion port pads, as they will act as stubs for the RDRAM; not digging them up may lead to the board not booting / possible instabilities in-game. Once all the necessary vias / traces have been scratched / tinned / dug up, the flex can be installed on the board. Once installed, run a magnet wire from the pad shown below and the bottom of R33 on the N64 (rambus clock output from the mx8330).

<img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/scratching.jpg" width=500> <img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/digging.jpg" width=500> <img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/installed.jpg" width=500>

## Testing
<img src="https://github.com/CrazyGadgetMods/AkiraFlex/blob/main/images/test.jpg" width=500>

## Credits
- [Akira](https://bitbuilt.net/forums/index.php?members/akira.1105/): [creating the original method for deadbugging the RDRAM termination circuit](https://bitbuilt.net/forums/index.php?threads/lockdown-64.4175/post-46301)
- [Noah](https://bitbuilt.net/forums/index.php?members/noah.1/): [inspiration from his unfinished Terminator 64 flex](https://bitbuilt.net/forums/index.php?threads/fusion64.3139/post-37558)
- [Cy](https://bitbuilt.net/forums/index.php?members/cy.7203/): [inspiration from his Terminator 64 flex](https://bitbuilt.net/forums/index.php?threads/ashida-64-working-title-n64-portable.5529/post-64147)
- [YveltalGriffin](https://github.com/mackieks): answering my many, many, *many* questions during my N64 anatomy deep-dive and helping me understand RDRAM / the Akira Method
- [BitBuilt](https://bitbuilt.net/): Being the best modding community out there!

## License
Solderpad Hardware License v2.1
