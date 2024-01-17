# syncmaster-P2250-nvidia-linux

AKA how I got native resolution working event though it's not reported by monitor.

This solution only works in Xorg.

Syncmaster P2250's ID: SAM0524

I found the EDID file in [this 13 year old thread](https://www.displaylink.org/forum/showthread.php?t=1287) without it I'd probably struggled with this for a while. Big s/o to rczig person. There is also [linuxhw/EDID](https://github.com/linuxhw/EDID/tree/master/Analog/Samsung) repo which stores EDID files, but the first one worked for me so I didn't bother. I also still dont know how to get the id of the device.

1. Acquire the EDID file from the repo
2. Store it somewhere
3. Add custom edid option to xorg as explained [here](https://nvidia.custhelp.com/app/answers/detail/a_id/3571/~/managing-a-display-edid-on-linux)

If you need more info/guidance open an issue I'm lazy ATM
