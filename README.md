# unicad
[![MELPA](https://melpa.org/packages/unicad-badge.svg)](https://melpa.org/#/unicad)

An elisp port of Mozilla Universal Charset Auto Detector

## About
unicad.el is an Elisp program port from Mozilla universal charset auto detector. After loading unicad in GNU Emacs, it can automatically detect multiple charsets, and you will never encounter garbled files in the future.

Following coding systems can be auto detected:
```
* (BOM detect)
* (ascii)
* multibyte coding systems:
 - gb18030 (gb2312)
 - big5
 - sjis
 - euc-jp
 - euc-kr
 - euc-tw
 - utf-8
 - utf-16le (also without signature)
 - utf-16be (also without signature)
* singlebyte coding systems:
 - greek
  > iso-8859-7
  > windows-1253
 - russian
  > koi8-r
  > windows-1251
  > iso-8859-5
  > ibm855
 - bulgarian
  > iso-8859-5
  > windows-1251
 - sjis (singlebyte only)
* latin-1
* latin-2
```

## Install

### with melpa
```
M-x package-install RET unicad RET
```

## Usage
``` elisp
(unicad-mode)
(unicad-mode 0)
```

M-x `unicad-mode`

## LICENSE
GPLv3

## Credits
`unicad` is written by [**Qichen Huang**](unicad.el@gmail.com). And [室见](https://github.com/ukari) is the MELPA maintainer of `unicad` .
