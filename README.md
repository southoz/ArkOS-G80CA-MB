# ArkOS-G80CA-MB

For God's sake, I brought another cheap Chinese game console!

It turned up, and as most know, buying a R36S from Aliexpress is like playing Russian Roulette.

Thanks to the great resources over at [Handheld Wiki](https://handhelds.wiki/R36S_Clones), I was able to identify that it was a G80CA-MB V1.2-20250422.

Obviously, the included firmware is less than optimal, so I went on the hunt.

Tried [ArkOS4Clone](https://github.com/lcdyk0517/arkos4clone) but the controller mapping needed a lot of work, and the Dreamcast performance was a bit hit and miss.

Downloaded [ArkOS for K36](https://github.com/AeolusUX/ArkOS-K36) and updated the DTB to Panel 8, which worked. The controls, however, were all over the place as this clone of a clone of a clone has been put together with gaffer tape using random parts.

Spent a minute trying to figure it out, then it all came flooding back like a bad case of PTSD.

Tried a number of external Wireless Adapters, and the OTG port doesn't provide enough power even for low-end wireless N adapters. The RL8188EU drivers are installed in the image so that dongle may work.

Decompiled multiple DTB files, attempting to find one with the function button, which is supposed to map to zed_keyboard SDL object rather than play_joystick. Updated the node with all different combinations of the GPIO pins, but was not able to get it to respond in evtest.

Panel 9 DTB Files are located [here](https://github.com/southoz/ArkOS-G80CA-MB/tree/main/DTB/Panel%209), however, I have no idea if they will work on a G80CA-MB V1.2 with Panel 9
