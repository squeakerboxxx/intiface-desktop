# Intiface Application

[![Build Status](https://dev.azure.com/nplabs/buttplug/_apis/build/status/intiface.intiface-desktop?branchName=master)](https://dev.azure.com/nplabs/buttplug/_build/latest?definitionId=5&branchName=master)

[![Patreon donate button](https://img.shields.io/badge/patreon-donate-yellow.svg)](https://www.patreon.com/qdot)
[![Discourse Forum](https://img.shields.io/badge/discourse-forum-blue.svg)](https://metafetish.club)
[![Discord](https://img.shields.io/discord/353303527587708932.svg?logo=discord)](https://discord.buttplug.io)
[![Twitter](https://img.shields.io/twitter/follow/buttplugio.svg?style=social&logo=twitter)](https://twitter.com/buttplugio)

Intiface is a set of applications and services for hosting sex toy
connections. Where [Buttplug](https://buttplug.io) is for developers,
Intiface is for users.

For those familiar with the development of
[Buttplug](https://buttplug.io) so far, you may have seen the
"Buttplug Server" and other programs. Intiface takes the place of the
Server program, and is the basis of UI/UX for Buttplug on both desktop
and mobile.

## Support The Project

If you find this project helpful, you
can
[support Nonpolynomial Labs projects via Patreon](http://patreon.com/qdot)!
Every donation helps us afford more hardware to reverse, document, and
write code for!

## Installation

Releases are available on the [Intiface Desktop Github Release
Site](https://github.com/intiface/intiface-desktop/releases).

Installers are available for:

- Windows 7-10 (Executable installer, tested on Windows 10)
- macOS (.Dmg file, Tested on 10.14)
- Linux (AppImage file, Tested on Debian 9)

The application will download the up-to-date device file and
engine for the operating system it is on.

## Linux Issues

To use Bluetooth LE on linux, you will need to run a couple of
commands after an engine is updated. Instructions here were adapted
from [https://github.com/noble/noble#running-without-rootsudo](https://github.com/noble/noble#running-without-rootsudo).

Run the following command:

```
sudo setcap cap_net_raw+eip ~/.config/Intiface/engine/IntifaceCLI
```

This grants the node binary cap_net_raw privileges, so it can start/stop BLE advertising.

Note: The above command requires setcap to be installed, it can be installed using the following:

- apt: `sudo apt-get install libcap2-bin`
- yum: `su -c \'yum install libcap2-bin\'`


## License

The Intiface Application is BSD 3-Clause licensed.

    Copyright (c) 2017-2019, Nonpolynomial Labs LLC
    All rights reserved.
    
    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions are met:
    
    * Redistributions of source code must retain the above copyright notice, this
      list of conditions and the following disclaimer.
    
    * Redistributions in binary form must reproduce the above copyright notice,
      this list of conditions and the following disclaimer in the documentation
      and/or other materials provided with the distribution.
    
    * Neither the name of the project nor the names of its
      contributors may be used to endorse or promote products derived
      from this software without specific prior written permission.
    
    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
    AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
    SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
    OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


