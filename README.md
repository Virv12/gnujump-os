# GnuJumpOS

## Build

To build `gnujump-os` run the following command in the project directory.
```sh
sudo rm -rf work && sudo mkarchiso -v .
```
The iso will be in the `out` directory.

## Run

To run `gnujump-os` run the following command in the project direcotory.
```sh
sudo qemu-system-x86_64 --enable-kvm -cpu host -m 4G -drive file=out/gnujump-os-$(date +'%Y.%m.%d')-x86_64.iso,format=raw
```

## TODO:

- configure grub
- add splash screen
- reduce ISO size
