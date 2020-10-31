# showem
Tool to monitor the progress of a parallel **emerge**(1) in Gentoo.

> 31 Oct 2020: sadly, due to legal obligations arising from a recent change in my 'real world' job, I must announce I am **standing down as maintainer of this project with immediate effect**. For the meantime, I will leave the repo up (for historical interest, and it may be of use to others); however, I plan no further updates, nor will I be accepting / actioning further pull requests or bug reports from this point. Email requests for support will also have to be politely declined, so, **please treat this as an effective EOL notice**.<br><br>For further details, please see my post [here](https://forums.gentoo.org/viewtopic-p-8522963.html#8522963).<br><br>With sincere apologies, sakaki ><

## Description
**showem** is a very simple utility script, which allows you to monitor the progress of a parallel **emerge**(1).

When invoked, it shows a split screen display, which updates once a second. The top part shows the tail of the current **Portage**(5) download log, and the lower part shows the tail of the most recent **Portage**(5) build log.

The download log display is cleared after 1 minute's inactivity; however, the build log is retained (even if stale) - this allows you to quickly see where a build has failed.

The path of the build log is displayed in the title bar of the window. If the window is resized, the display is adapted automatically to fit; however, a minimum size of 80 columns and 24 rows is required.

Exit **showem** using Ctrl-c, when done.

## Installation

**showem** is best installed (on Gentoo) via its ebuild, available as part of the **sakaki-tools** [overlay](https://github.com/sakaki-/sakaki-tools).
Full instructions are provided as part of the [**Sakaki's EFI Install Guide**](https://wiki.gentoo.org/wiki/Sakaki's_EFI_Install_Guide) tutorial, on the Gentoo wiki.
