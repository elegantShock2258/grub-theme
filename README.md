# rEFInd Metal Theme

Theme for the [(U)EFI rEFInd boot manager](https://sourceforge.net/projects/refind/).  This theme has a metal
background, with a "glowing" blue outline logo for the OS selections.  Almost every icon of the original theme has been
replaced.

![Boot Selection](https://i.imgur.com/tqCDzpB.jpg)

![Function Selection](https://i.imgur.com/WUlfdsW.jpg)

## Installation

This theme requires rEFInd to be installed.  Change directory to the rEFInd directory, where `refind_x64.efi` is
located on your system (on Linux, usually located at `/boot/EFI/refind` or `/boot/efi/EFI/refind`) and, if necessary,
create the subdirectory `themes`:

```console
foo@bar:~$ cd /boot/EFI/refind
foo@bar:refind$ mkdir themes
```

Clone the metal directory to the themes directory:

```console
foo@bar:refind$ git clone https://gitlab.com/perthshiretim/refind-metal-theme.git themes/metal
```

Include the `metal/theme.conf` to `refind.conf` (located in the rEFInd directory):

```console
foo@bar:refind$ echo -e "\ninclude themes/metal/theme.conf\n" >> refind.conf
```

The file `theme.conf` assumes a resolution of 1920x1080 for your monitor. If necessary, change this by modifying the
first line of `theme.conf` to something appropriate (self-explanatory).

## Licence Information

Attribution and licence information for the original icons is in the file COPYRIGHT.
