# Boo for [GRUB](https://gnu.org/software/grub/)

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)[![Arch](https://img.shields.io/badge/Arch%20Linux-1793D1?logo=arch-linux&logoColor=fff&style=for-the-badge)](https://aur.archlinux.org/packages/boo-grub-git)

> A dark theme for [GRUB](https://gnu.org/software/grub/).

![Screenshot](./assets/grub.png)

## Compatibility
It should be compatible with all linux distros that use grub.

## Installation

### AUR

For Arch users, the theme is available from the AUR [here](https://aur.archlinux.org/packages/boo-grub-git).

1. Install it with your favorite AUR helper: `paru boo-grub-git`

2. Follow steps 3. and 4. given below.

### Manually

1. Clone this repo or download the .zip

```bash
$ git clone https://github.com/PROxZIMA/boo-grub.git
$ cd boo-grub
```

2. Copy the whole `boo` directory to grub themes

```bash
$ sudo cp -r boo /usr/share/grub/themes
```

3. Edit grub config file

```bash
$ sudo vim /etc/default/grub
```

change `#GRUB_THEME=` to `GRUB_THEME="/usr/share/grub/themes/boo/theme.txt"`

4. Update grub using

```bash
$ sudo grub-mkconfig -o /boot/grub/grub.cfg
```

5. Reboot and voila

## Potential problems and solutions

Never had one but still refer to the following article.

https://www.jeremymorgan.com/tutorials/linux/how-to-reinstall-boot-loader-arch-linux/


## Credit

- [Ghost profile](https://www.flaticon.com/free-icon/ghost_2085034)
- [Tokyo-Night GRUB](https://github.com/mino29/tokyo-night-grub/)

## License

[MIT License](./LICENSE)
