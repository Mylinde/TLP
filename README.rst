TLP - Optimize Linux Laptop Battery Life
========================================
TLP is a feature-rich utility for Linux, saving laptop battery power
without the need to delve deeper into technical details.

TLP’s default settings are already optimized for battery life, so you may just
install and forget it. Nevertheless TLP is highly customizable to meet your specific
requirements.

Settings are organized into three customizable profiles *performance* (AC),
*balanced* (BAT) and *power-saver* (SAV), allowing to adjust between savings
and performance independently for battery and AC operation.

*Version 1.9* introduces the (optional) TLP profiles daemon (**tlp-pd**), which
enables choosing between the three profiles with a mouse click. Together with TLP
as the backend it **replaces power-profiles-daemon** by implementing the same
D-Bus API that major Linux desktop environments like GNOME, KDE and Cinnamon
already use for switching power profiles.

In addition TLP can enable or disable Bluetooth, NFC, Wi-Fi and WWAN radio
devices on boot and when connecting/removing the LAN cable.

For ThinkPads and other supported laptops it provides a unified approach to
battery charge thresholds.


**Dynamic SAV Daemon** *(Difference to upstream TLP)*
-------------
This fork includes an additional optional **tlp-dyn-saver** daemon that
dynamically adjusts power-saver profile parameters based on system workload.
It monitors CPU utilization and automatically switches between three power
levels (low/medium/high) for PLATFORM_PROFILE, CPU_ENERGY_PERF_POLICY, and
PCIE_ASPM settings. This enables automatic optimization without manual
intervention - maximizing battery life during idle periods while maintaining
responsiveness when needed. The daemon is disabled by default.

Documentation
-------------
Read the full documentation at the website `<https://linrunner.de/tlp>`_.

For a summary of how TLP works and its features see
`Introduction <https://linrunner.de/tlp/introduction>`_.

Installation
------------
TLP packages are available for all major Linux distributions:
`Installation <https://linrunner.de/tlp/installation>`_.

Settings
--------
Settings are organized into two profiles, enabling you to adjust between savings
and performance independently for battery (BAT) and AC operation.

Refer to `Settings <https://linrunner.de/tlp/settings/introduction>`_ to learn
how to customize the configuration if desired.

Support
-------
Please visit your favorite Linux community for help and support questions.
Make shure to check `Support <https://linrunner.de/tlp/support>`_ first.

Bug reports
-----------
Refer to the
`Bug Reporting Howto <https://github.com/linrunner/TLP/blob/master/.github/Bug_Reporting_Howto.md>`_.

Contribute
----------
Contributing is not only about coding. Volunteers helping with support, testing
and documentation are always welcome!

See `Contributing <https://linrunner.de/tlp/contribute>`_.
