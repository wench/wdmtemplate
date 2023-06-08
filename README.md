# wdmtemplate
A simple Open Source Windows WDM driver template
by Alexis Ryan <the.wench@wenchy.net>

This source code is intended to be used to create Open Source Drivers for Windows because the license for the samples included with the Windows DDK and WDK is not suitable for use with Open Source drivers.

This Source code is not a full driver. It contains the basics needed for a PnP WDM driver, irps for driver functionality needs to be written. It has been written for Windows NT based operating systems (Windows 2000 and newer). It has not been Written to support Windows 98 or Windows Me. It may work for those but everything is completely untested. The intent is really only for 32 bit support but the code should be 64 bit safe. The code should be suitable for a feature driver or filter driver. A bus driver will probably need changes. It wont be suitable for use to create other driver types like NDIS or KMDF.

The source contains stubs for all unimplemented IRPs as well as basic Driver and FDO structs that can be extended as needed. Remember to set a unique device object name and DOSDevice Alias (these are set by a Macro)

I will not offer any support on how to develop a driver beyound what is in the source and this document. I mostly created this for myself to use as a base to create some fully featured drivers for some retro hardware that didn't have suitable Windows 2000 drivers and thought it would be a useful community project by itself.
