# Passive Scan on CC3100 for IoT / Documentation

The [Silent Dragonfly](https://github.com/silent-dragonfly) team has been
created for implementing passive scan for CC3100, which driver apparently is not
supported this feature ([TI forums](http://e2e.ti.com/support/wireless-connectivity/wifi/f/968/p/684381/2521400)).
The project are going as *Research Project 1* of SNE Innopolis course
([os3.su](http://os3.su/)).


This [docs](https://github.com/silent-dragonfly/docs) repository are contained
the main notes and documentation for this project.

## Equipment

- CC3100BOOST ([ti.com](http://www.ti.com/tool/CC3100BOOST))
- CC31XXEMUBOOST ([ti.com](http://www.ti.com/tool/CC31XXEMUBOOST))

## Private Area

Since we are using the [CC3100 SDK](www.ti.com/tool/CC3100SDK), we can use, but
can not openly distribute this materials. If possible we are directly referring
to the TI website. Or put that materials on our website, which are accessible only
by team members.

As a third party, you can treat links to the `https://passive-scan.std12.os3.su/`
as `C:\TI\CC3100SDK_1.3.0\cc3100-sdk\docs` local folder, if you install the SDK
to the default location.

## Theory

- Notes about [Physic layer](./IEEE802.11/phy.md) (PHY)
- [Connection Initiation](./IEEE802.11/connection-initiation.md) - Scan, Authentication, Association
- [Frame formats information](./IEEE802.11/frame-formats.md)

## Technical stages

1. [Setting up the workstation](00-setup-workstation/set-up-workstation.md)
2. [Print CC3100 Information](01-print-cc3100-information/print-cc3100-information.md)
3. [Using devices](02-using-cc3100/using-cc3100-devices.md)

## Miscellaneous

- [Cookbook](cookbook.md) - links and short code-snippets, which are useful for
research and development.
- [Raw resources](raw-sources.md) - articles and/or sources that should be
explored and sorted.
