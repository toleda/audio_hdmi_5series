audio_hdmi_5series
============
OS X AMD/Nvidia HDMI Audio dsdt edits

This guide enables OS X HDMI audio on Intel based 5 Series motherboards with a bootable clean install of OS X.  Supported HDMI audio graphics systems are AMD discrete graphics cards (HD5xxx, HD6xxx and HD7xxx) and Nvidia discrete graphics cards (4xx, 5xx, 6xx and 7xx).  The Optimized AppleHDA.kext supports HDMI audio and Realtek audio codecs (ALC885, ALC887, ALC888, ALC889, ALC892 and ALC898) for onboard audio.  The native ML AppleHDA.kext supports only HDMI audio when configured properly. In Mountain Lion, the Optimized AppleHDA.kext supports 1 Audio_ID for HDMI and Realtek onboard audio:
Audio_ID: 1 supports AMD/Nvidia HDMI and 3, 5 and 6 port ALC8xx onboard audio  

Note
1. Native ML AppleHDA.kext, use Audio_ID: 1, for HDMI audio/no onboard audio

OS X versions supported
1. Mavericks.10.9 and newer
2. Mountain Lion/10.8.2 and newer

More Information
1. Mountain Lion: Optimized AppleHDA for Realtek ALC8xx
http://www.tonymacx86.com/audio/76202-mountain-lion-optimized-applehda-realtek-alc8xx.html#post472375
2. Mountain Lion HDMI Audio - AMI DSDT
http://www.tonymacx86.com/hdmi-audio/70762-mountain-lion-hdmi-audio-ami-dsdt.html
3. Mountain Lion HDMI Audio - Award DSDT
http://www.tonymacx86.com/hdmi-audio/70758-mountain-lion-hdmi-audio-award-dsdt.html

ML 5 Series HDMI Audio dsdt edits
1. MaciASL - http://sourceforge.net/projects/maciasl/?source=navbar
2. Configuration: MaciASL/Preferences/Sources/+/  (copy/paste URL, don't click)
3. URL: https://raw.github.com/toleda/audio_hdmi_5series/master
4. Download/ZIP: https://github.com/toleda/audio_hdmi_5series

Usage
1. If no dsdt. extract dsdt, MaciASL/File/New from ACPI/DSDT
2. MaciASL/File/Open dsdt
3. MaciASL/Patch/toleda_hdmi_5series/Select Patch/es
4. MaciASL/Patch/Apply (Repeat, as necessary) 
5. MaciASL/Patch/Close
6. MaciASL/Compile
7. MaciASL/File/Save As…/ACPI Machine Language Binary/dsdt.aml

Installation - edited dsdt.aml to Extra
1. MaciASL/File/Save As…/ACPI Machine Language Binary/Extra/dsdt.aml (add extension)

Problem Reporting
1. Motherboard/BIOS version/processor/graphics/OS and version
2. Copy of dsdt (if edited)
3. Copy of HDMI audio SSDT (if installed)
4. Copy of IORegistryExplorer

Troubleshooting/Post w/attachments 2-4, above
1. Mavericks/10.9
1a. http://www.tonymacx86.com/hdmi-audio/112469-mavericks-hdmi-audio-applehda.html
1b. http://www.insanelymac.com/forum/topic/292999-mavericks-applehda-hdmi-audio/
2. Mountain Lion/10.8
2a.http://www.tonymacx86.com/hdmi-audio/70762-mountain-lion-hdmi-audio-ami-dsdt.html
2b. http://www.insanelymac.com/forum/topic/291103-mountain-lion-hdmi-audio/

Guides:
1. Nehalem/1st Generation Core Processors/5 Series motherboards (No HD Graphics)
1a. [Guide]-5_series-hdmi_audio_dsdt_edits_v1.1.pdf.zip
1b. Patches 
    5s1. AMI-BIOS-AMD-Nvidia-5_Series-A1 - AMD/Nvidia HDMI audio dsdt edits
    5s2. Award-BIOS-AMD-Nvidia-5_Series-A1 - AMD/Nvidia HDMI audio dsdt edits

toleda
https://github.com/toleda/audio_hdmi_5series
Patches
README.txt