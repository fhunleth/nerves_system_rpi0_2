# Changelog

This project does NOT follow semantic versioning. The version increases as
follows:

1. Major version updates are breaking updates to the build infrastructure.
   These should be very rare.
2. Minor version updates are made for every major Buildroot release. This
   may also include Erlang/OTP and Linux kernel updates. These are made four
   times a year shortly after the Buildroot releases.
3. Patch version updates are made for Buildroot minor releases, Erlang/OTP
   releases, and Linux kernel updates. They're also made to fix bugs and add
   features to the build infrastructure.

## v1.23.1

This is a bug and security fix update. It should be a low risk upgrade.

* Fixes
  * Fix CTRL+R over ssh

* Updated dependencies
  * [nerves_system_br v1.23.2](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.23.2)
  * [Buildroot 2023.02.2](https://lore.kernel.org/buildroot/87y1je6wva.fsf@48ers.dk/T/)

## v1.23.0

This is a major update that brings in Erlang/OTP 26, Buildroot 2023.02.2, Linux
6.1, and Raspberry Pi firmware updates.

* New features
  * The Raspberry Pi cameras now work with libcamera. The libcamera apps are
    included. See the [Raspberry Pi Camera docs](https://www.raspberrypi.com/documentation/computers/camera_software.html).
  * CA certificates are included for OTP 26.

* Changes
  * The `start.elf` and `fixup.dat` files were renamed to `start4.elf` and
    `fixup4.dat` to be more consistent with the RaspberryPi OS naming.

* Updated dependencies
  * [nerves_system_br v1.23.1](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.23.1)
  * [Buildroot 2023.02.2](https://lore.kernel.org/buildroot/87wn03ifbl.fsf@48ers.dk/T/)
  * [Erlang/OTP 26.0.2](https://erlang.org/download/OTP-26.0.2.README)
  * Linux 6.1.21 (Raspberry Pi Linux tag 1.20230405)

## Previous releases

This is a fork of [nerves_system_rpi3a](https://github.com/nerves-project/nerves_system_rpi3a).
See that project for previous history. The version numbers were kept for convenience.

