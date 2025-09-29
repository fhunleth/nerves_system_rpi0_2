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

## v1.31.4

* Changes
  * Synchronize and fix Raspberry Pi camera settings

## v1.31.3

This is an important security/bug fix that addresses Erlang CVEs for the ssh
module (see Erlang release notes).

* Package updates
  * [nerves_system_br v1.31.7](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.31.7). Also
    see [nerves_system_br v1.31.6](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.31.6)

* Important derived package updates
  * [Erlang/OTP 27.3.4.3](https://erlang.org/download/OTP-27.3.4.3.README.md)
  * [Buildroot 2025.02.6](https://lore.kernel.org/buildroot/b051d400-debc-4269-975a-b2992eed8d61@rnout.be/T/)

## v1.31.2

This is a security/bug fix release.

* Package updates
  * [nerves_system_br v1.31.5](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.31.5)

* Important derived package updates
  * [Erlang/OTP 27.3.4.2](https://erlang.org/download/OTP-27.3.4.2.README.md)
  * [fwup 1.13.2](https://github.com/fwup-home/fwup/releases/tag/v1.13.2)

## v1.31.1

This is a security/bug fix release.

* Package updates
  * [Erlang/OTP 27.3.4.1](https://erlang.org/download/OTP-27.3.4.1.README.md)
  * [Buildroot 2025.02.3 (fixed 2025.02.2)](https://lore.kernel.org/buildroot/49d039c0-8121-4a91-8a69-889376f85c71@rnout.be/T/)
  * Raspberry Pi WiFi firmware 1:20240709-2~bpo12+1+rpt3
  * [rpi-libcamera v0.5.0+rpt20250429](https://github.com/raspberrypi/libcamera/releases/tag/v0.5.0%2Brpt20250429)
  * rpicam-apps 1.7.0
  * [erlinit 1.14.3](https://github.com/nerves-project/erlinit/releases/tag/v1.14.3)
  * [fwup 1.13.0](https://github.com/fwup-home/fwup/releases/tag/v1.13.0)

## v1.31.0

This is a major Buildroot update.

Please see the [nerves_system_br v1.31.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.31.0)
for additional information if you've forked this system.

* Updated dependencies
  * [Buildroot 2025.02.1](https://lore.kernel.org/buildroot/60b8483c-b717-41ce-a406-bceb71c3a089@rnout.be/T/)

## v1.30.1

This is a security/bug fix update.

* Updated dependencies
  * [Erlang/OTP 27.3.3](https://erlang.org/download/OTP-27.3.3.README)
  * [nerves_system_br v1.30.1](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.30.1)

## v1.30.0

This is a major Buildroot update.

Please see the [nerves_system_br v1.30.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.30.0)
for upgrade instructions if you've forked this system.

* Changes
  * Add REUSE compliance to help improve OSS copyright and licensing accuracy
  * Update Raspberry Pi libraries and firmware to latest releases

* Updated dependencies
  * [Erlang/OTP 27.3](https://erlang.org/download/OTP-27.3.README.md)
  * [Buildroot 2024.11.2](https://lore.kernel.org/buildroot/87v7t3nyls.fsf@dell.be.48ers.dk/T/)
  * Linux 6.6.74 (Raspberry Pi 1.20250127 release)
  * rpicam-apps 1.5.3
  * rpi-libcamera v0.3.2+rpt20241119
  * rpi-distro-firmware-nonfree 1:20230625-2+rpt3

## v1.29.1

This is a security/bug fix update.

* Updated dependencies
  * [nerves_system_br v1.29.3](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.29.3)
  * [Buildroot 2024.08.3](https://lore.kernel.org/buildroot/874j3e17ek.fsf@dell.be.48ers.dk/T/)
  * [Erlang/OTP 27.2](https://erlang.org/download/OTP-27.2.README)
  * Linux 6.6.64 with the Raspberry Pi and PREEMPT_RT patches
  * [fwup v1.12.0](https://github.com/fwup-home/fwup/releases/tag/v1.12.0)

## v1.29.0

This is a major Erlang and Buildroot update.

Please see the [nerves_system_br v1.29.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.29.0)
for upgrade instructions if you've forked this system.

* Changes
  * Applied and enabled the Real-Time Linux patch set, PREEMPT_RT. Please see
    write-ups on the web for benefits and how to use. The impact of this patch
    shouldn't be noticeable to most Nerves users.
  * Switch CPU frequency governor from conservative to the more modern
    schedutil. See [LWN article](https://lwn.net/Articles/682391/) for details.
  * Upgrade `fwup-revert.conf` to more capable `fwup-ops.conf`

* Updated dependencies
  * [nerves_system_br v1.29.1](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.29.1)
  * [Buildroot 2024.08.2](https://lore.kernel.org/buildroot/871pzex7gn.fsf@dell.be.48ers.dk/T/)
  * Linux 6.6.51 (Raspberry Pi stable_20241008 release)

## v1.28.1

This is a security/bug fix update.

* Changes
  * Enable libdrm so that camera preview works

* Updated dependencies
  * [nerves_system_br v1.28.3](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.28.3)
  * [Buildroot 2024.05.2](https://lore.kernel.org/buildroot/87zfpfh147.fsf@dell.be.48ers.dk/T/)
  * [Erlang/OTP 27.0.1](https://erlang.org/download/OTP-27.0.1.README)

## v1.28.0

This is a major Erlang and Buildroot.

Please see the [nerves_system_br v1.28.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.28.0)
for upgrade instructions if you've forked this system.

* Changes
  * Elixir 1.17 and Erlang/OTP 27 support
  * Reduce copy/pasted definitions in the `fwup.conf` by extracting them to
    `fwup_include/fwup-common.conf`. (No functional changes)

* Fixes
  * The serial numbers returned by `Nerves.Runtime.serial_number/0` now contain
    the whole serial number. If you forked this system, check the
    `boardid.config` and `erlinit.config` for the changes and to keep the
    hostname the same.

* Updated dependencies
  * Linux 6.6.31 (Raspberry Pi stable_20240529 release)
  * [nerves_system_br v1.28.1](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.28.1)
  * [Buildroot 2024.05](https://lore.kernel.org/buildroot/87bk46tjk2.fsf@dell.be.48ers.dk/T/)
  * [Erlang/OTP 27.0](https://erlang.org/download/OTP-27.0.README)

## v1.27.1

This is a security/bug fix update.

* Package updates
  * [Erlang/OTP 26.2.5](https://erlang.org/download/OTP-26.2.5.README)
  * [Buildroot 2024.02.1](https://lore.kernel.org/buildroot/87jzlp9u5e.fsf@48ers.dk/T/)

## v1.27.0

This is a major Buildroot update.

Please see the [nerves_system_br v1.27.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.26.0)
for upgrade instructions if you've forked this system.

* Changes
  * The `libcamera` and `rpicam_apps` packages have been replaced with the
    Raspberry Pi-forked versions for better compatibility. Please see
    `nerves_system_br` release notes.
  * Add back `CONFIG_RASPBERRYPI_GPIOMEM` to support the `dht` library.

* Updated dependencies
  * Linux 6.1.73 (Raspberry Pi 20240124 release)
  * [nerves_system_br v1.27.0](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.27.0)
  * [Buildroot 2024.02](https://lore.kernel.org/buildroot/87msrczp4z.fsf@48ers.dk/)
  * [Erlang/OTP 26.2.3](https://erlang.org/download/OTP-26.2.3.README)

## v1.26.0

This is a major Buildroot update.

Please see the [nerves_system_br v1.26.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.26.0)
for upgrade instructions if you've forked this system.

* New features
  * Add the imx296 overlays for the Raspberry Pi Global Shutter Camera

* Updated dependencies
  * [Erlang/OTP 26.2.2](https://erlang.org/download/OTP-26.2.2.README)
  * [nerves_system_br v1.26.1](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.26.1)
  * [Buildroot 2023.11.1](https://lore.kernel.org/buildroot/87cyu2k2gu.fsf@48ers.dk/T/)

## v1.25.1

This is a security/bug fix update.

*  Package updates
  * [Erlang/OTP 26.2.1](https://erlang.org/download/OTP-26.2.1.README)
  * [nerves_heart 2.3.0](https://github.com/nerves-project/nerves_heart/releases/tag/v2.3.0)

## v1.25.0

This is a major Buildroot and toolchain update that also adds support for using
Scenic without customizing the system.

Please see [nerves_system_br v1.25.0 release notes](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.25.0)
for upgrade instructions if you've forked this system.

* New features
  * Add libcairo for [Scenic](https://github.com/ScenicFramework/scenic) support

* Updated dependencies
  * [nerves_system_br v1.25.2](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.25.2)
  * [Buildroot 2023.08.4](https://lore.kernel.org/buildroot/87o7f6t7fs.fsf@48ers.dk/T/)
  * [Erlang/OTP 26.1.2](https://erlang.org/download/OTP-26.1.2.README)

## v1.24.1

This is a security/bug fix update.

* Package updates
  * [nerves_system_br v1.24.1](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.24.1)
  * [Erlang/OTP 26.1.1](https://erlang.org/download/OTP-26.1.1.README)
  * [Buildroot 2023.05.3](https://lore.kernel.org/buildroot/87h6ngup34.fsf@48ers.dk/T/)

## v1.24.0

This is a Buildroot version update that appears to mostly contain bug and
security fixes. It should be a low risk upgrade from v1.23.2.

* Updated dependencies
  * [nerves_system_br v1.24.0](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.24.0)
  * [Buildroot 2023.05.2](https://lore.kernel.org/buildroot/87ledrkrpp.fsf@48ers.dk/T/), [2023.05.1](https://lore.kernel.org/buildroot/87351m8qm4.fsf@48ers.dk/T/), [2023.05](https://lore.kernel.org/buildroot/87r0qn2c77.fsf@48ers.dk/T/)
  * [Erlang/OTP 26.1](https://erlang.org/download/OTP-26.1.README)

## v1.23.2

* Updated dependencies
  * [nerves_system_br v1.23.3](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.23.3)

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

