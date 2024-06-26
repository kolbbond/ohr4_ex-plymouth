# ohr4_ex for [Plymouth](https://gitlab.freedesktop.org/plymouth/plymouth)

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)[![Arch](https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff&style=for-the-badge)](https://aur.archlinux.org/packages/proxzima-plymouth-git)

> A techno [Plymouth](https://gitlab.freedesktop.org/plymouth/plymouth) theme made from other themes 

# add our own gif for the github
#| Boot Screen | Shutdown Screen |
#| :-------------: | :-------------: |
#| ![Boot Screen](./assets/boot.gif)  | ![Shutdown Screen](./assets/shut.gif)  |

## Installation

### AUR

# add a package?
#For Arch users, the theme is available from the AUR [here](https://aur.archlinux.org/packages/proxzima-plymouth-git).


### Manually

#### Dependencies

- plymouth

> **Note**
>
> `plymouth-x11` is required to preview the theme without rebooting.

1. Clone this repo or download the .zip

```bash
$ git clone https://github.com/kolbbond/ohr4_ex-plymouth.git
```

2. Copy the whole `ohr4_ex` directory to plymouth themes

```bash
$ sudo cp -r ohr4_ex /usr/share/plymouth/themes
```

3. Follow the steps based on your distribution

    - Arch based distros
    ```
    # check if theme exist in dir
    sudo plymouth-set-default-theme -l

    # optionally you can test the theme by running the script given in repo (plymouth-x11 required)
    sudo ./preview.sh 

    # now set the theme (ohr4_ex, in this case) and rebuilt the initrd
    sudo plymouth-set-default-theme -R ohr4_ex
    ```

4. Reboot and voila

## Configuration

## Potential problems and solutions

Never had one but still refer to the following articles.

- https://wiki.archlinux.org/title/plymouth
- https://wiki.ubuntu.com/Plymouth

For scripting: https://www.freedesktop.org/wiki/Software/Plymouth/Scripts/

## Credits

- [Roger Truttmann](https://twitter.com/RogerTruttmann): The creator of the animation 🙌. Follow him on [Twitter](https://twitter.com/RogerTruttmann), [Github](https://github.com/ROGERdotT) and [Lottiefiles](https://lottiefiles.com/roger.t).
- [Archcraft](https://archcraft.io/): The main logo is designed by [@adi1090x](https://github.com/adi1090x).
- [showplymouth.sh](https://github.com/adi1090x/plymouth-themes): Made by [@adi1090x](https://github.com/adi1090x).
- [Proxzima](https://github.com/proxzima/)
- [plymouth themes](https:/github.com/plymouth-themes)

## License

#[GPLv3 License](LICENSE).
