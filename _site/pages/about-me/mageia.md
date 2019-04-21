Mageia was surprisingly a rather pleasant experience for me. Everything 'just worked' rather well with it, I have noticed no bugs in the few days I have used it so far. I personally think it would probably make for a great system to run on a desktop PC with hardware entirely compatible with open-source software (no need for proprietary drivers, not even for better performance) used by the technologically-inept, or at least less skilled, so long as their computing needs are fairly basic. As expected, based on my virtual machine experience with it and basic research I have done on it, its software was a little outdated (e.g. using KDE Plasma LTS which is presently 5.8.x, as well as Firefox ESR), but still well-tested, usable and stable.

The problems I noticed with it was what I expected, namely that Broadcom drivers were not pre-installed, neither in the live session nor fresh installation. Although this problem, like usual, is simple to fix, merely install them and they are ready to go. That and I must admit I am not the biggest fan of urpmi, thankfully there is DNF pre-installed which I favour as its syntax is simpler.

Arch Linux's GRUB bootloader (as I triple booted Arch Linux / Gentoo Linux / Void Linux at the time and was using a fourth partition to test distributions out on ) did not play nice with it, it used an old kernel (the one Mageia 6 comes with in a fresh install) of Mageia's (for which I had not installed Broadcom wireless) as the default instead of the latest kernel (and yes I had updated the configuration file with `grub-mkconfig -o /boot/grub/grub.cfg` since the install of the newer kernel). The newer kernel was in the advanced options list of Mageia, but having to go there every time I wanted to boot it was irritating.