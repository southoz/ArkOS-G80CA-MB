# ArkOS-G80CA-MB

For God's sake, I brought another cheap Chinese game console!

It turned up, and as most know, buying a R36S from Aliexpress is like playing Russian Roulette.

Thanks to the great resources over at [Handheld Wiki](https://handhelds.wiki/R36S_Clones), I was able to identify that it was a G80CA-MB V1.2-20250422.

Obviously, the included firmware is less than optimal, so I went on the hunt.

Tried [ArkOS4Clone](https://github.com/lcdyk0517/arkos4clone); it worked, but in the end, it wasn't supported, and the screen was banding.

Downloaded [ArkOS for K36](https://github.com/AeolusUX/ArkOS-K36) and updated the DTB to Panel 8, which worked the controls; however, they were all over the place.

Spent a minute trying to figure it out, then it all came flooding back like a bad case of PTSD.

Image is the archived [ArkOS-K36](https://github.com/AeolusUX/ArkOS-K36) with an updated DTB and some controller tweaks to make it work with the G80CA-MB

Spent a bit of time on external Wireless Adapters, and the OTG port doesn't provide enough power even for low-end wireless N adapters. The RL8188EU drivers are installed in the image so that dongle may work.

