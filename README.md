# Hackintosh EFI for Matebook 14(2019)

This EFI can be used to install Big Sur beta I-IV, the remaining versions have not been tested.

It is also known that the EFI also supports the installation of the version Catalina(10.15.X) tested on Matebook 13(2020).

This EFI includes the itlwm Wi-Fi driver, and automatic connection when starting up can be realized through modified the itlwm.kext/Contents/Info.plist.

But second generation devices still need itlwmx drivers.

Problems encountered on Matebook 14:

a) Whether new installation is supported has not been tested.

b) Problems with indirect upgrade:

  i.During the first restart from beta II to beta IV, there may be no reading. You need to wait 15-20 minutes for the second restart very patiently;
  
  ii.During the second restart, the stuck progress bar or no progress bar may appear. It can be solved by adding parameters vsmcgen=1 and -v in boot -args.
  
  iii.Use after config.plist You can, and change the value of showpicker to false to close the selection menu.

c) The popular white washing three-Code Course in the Internet is not applicable to this EFI, and direct replacement of PlatformInfo may cause the computer to fail to turn on.

d) And the last, the order of ALT and Win keys is opposite, but fortunately it can be modified in Settings >> Keyboard >> Modifier Key.


If you have any questions, you can leave a message on my Wechat public platform.
