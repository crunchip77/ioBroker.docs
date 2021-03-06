---
translatedFrom: en
translatedWarning: 如果您想编辑此文档，请删除“translatedFrom”字段，否则此文档将再次自动翻译
editLink: https://github.com/ioBroker/ioBroker.docs/edit/master/docs/zh-cn/adapterref/iobroker.cul/README.md
title: ioBroker.cul
hash: K4rCOBSVFqE1jD3svv7aukvEal1t2fI6QVtX90V21KE=
---
![商标](../../../en/adapterref/iobroker.cul/admin/busware.jpg)

![安装数量](http://iobroker.live/badges/cul-stable.svg)
![NPM版本](http://img.shields.io/npm/v/iobroker.cul.svg)
![资料下载](https://img.shields.io/npm/dm/iobroker.cul.svg)
![测验](https://travis-ci.org/ioBroker/ioBroker.cul.svg?branch=master)
![NPM](https://nodei.co/npm/iobroker.cul.png?downloads=true)

＃ioBroker.cul
ioBroker适配器可通过[CUL](http://busware.de/tiki-index.php?page=CUL)/[ulf](http://culfw.de)控制FS20，Max！，HMS和其他设备。取决于https://github.com/hobbyquaker/cul

**此适配器使用Sentry库自动向开发人员报告异常和代码错误。**有关更多详细信息以及如何禁用错误报告的信息，请参见[哨兵插件文档](https://github.com/ioBroker/plugin-sentry#plugin-sentry)！ Sentry报告从js-controller 3.0开始使用。

##支持的设备
-* EM *-EM1000WZ，EMWZ
-* FS20 *，含ESA1000 / 2000
-* HMS *-HMS100-TF，HMS100-T，HMS100-WD，RM100-2，HMS100-TFK，HMS100-MG，HMS100-CO，HMS100-FIT
-* MORITZ *-MAX！
-* WS *-KS300TH，S300TH，WS2000 / WS7000

＃＃ 如何
###例如，将命令发送到FS20设备。的JavaScript
```sendTo("cul.0", "send", {"protocol":"FS20", "housecode":"A1B2", "address":"01", "command":"00"});```

###使用JavaSript发送原始命令（例如，发送到InterTechno设备）
```sendTo("cul.0", "sendraw", {"command": 'is0FFFFF0FFFFF'});```

此命令使用此适配器的CUL库向设备发送命令。
基于Javascript / Node.js的Busware CUL USB / culfw适配器

## Changelog

### 1.3.3 (2020-09-25)
* (EvilEls) Added raw command support with cul.write()

### 1.3.2 (2020-08-23)
* (Apollon77) check that all needed objects are existing on start (Sentry IOBROKER-CUL-C)
* (Apollon77) fix Moritz device crash case (Sentry IOBROKER-CUL-7)

### 1.3.1 (2020-07-26)
* (Apollon77) make sure connection check do not crash adapter (Sentry IOBROKER-CUL-3)
* (Apollon77) crashes preventd (Sentry IOBROKER-CUL-5, IOBROKER-CUL-8)

### 1.3.0 (2020-07-20)
* (Apollon77) Really update dependencies and Serialport

### 1.2.2 (2020-04-30)
* (Apollon77) Update dependencies/Serialport 

### 1.2.1 (2020-03-18)
* (bluefox) Changed license from non SPDX conform 
    "GPL-2.0" to "GPL-2.0-or-later"

### 1.2.0 (2020-02-10)
* (MK-2001) Sending of FS20 cmdRAW possible or via sendTo as described in the readme
* (Bluefox) Refactoring

### 1.1.0 (2020-01-04)
* (foxriver76) removed usage of adapter.objects

### 1.0.0 (2019-05-15)
* (Apollon77) Support for nodejs 12 added, nodejs 4 is no longer supported!

### 0.4.0 (2018-03-07)
* (Apollon77/Michael Lorenz) Optimizations for nanoCul, Support for ESA devices

### 0.3.0 (2018-01-23)
* (Apollon77) Upgrade Serialport Library

### 0.2.2 (2017-01-23)
* (bluefox) use new npm cul module

### 0.2.0 (2017-01-21)
* (bluefox) Add raw data state

### 0.1.1 (2017-01-14)
* (bluefox) Use newer version of cul module

### 0.1.0 (2016-11-01)
* (bluefox) Update cul package

### 0.0.4 (2015-04-16)
* (bluefox) update package.json

### 0.0.3 (2015-03-03)
* (bluefox) try to bring the adapter to state of the art

## License

[Licensed under GPLv2](LICENSE) Copyright (c) 2014-2020 hobbyquaker