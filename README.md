------------------------
the Virtual USB Analyzer
------------------------
GitHub Edition

Hello! This is an old project from 2005 that I just now (2014) imported from SourceForge to GitHub. I wrote this way back when I worked at VMware, and it uses many obsolete GUI libraries that are only available for Linux these days. But it still runs nicely in an Ubuntu VM, and this repo now exists as an opportunuity to gradually modernize a tool many people including myself still find useful.

Fow now I'll leave you with a few notes:

* The version of vusb-analyzer in Ubuntu is too old to support the log format used by current releases of VMware products. Use this version instead.
* Modern VMware releases also include an automatic log throttling feature that can suck if you're trying to record a pristine log of some operation's traffic. For tasks like this, I find the following config options helpful:

```
monitor = "debug"
usb.analyzer.enable = TRUE
usb.analyzer.maxLine = 8192
mouse.vusb.enable = FALSE
log.throttleBytesPerSec = 100000000
```

–Micah

---------------------

This is a GUI tool for analyzing logs of traced USB
communications. For more information, see the project's web page:

http://vusb-analyzer.sourceforge.net

The Virtual USB Analyzer is distributed under the MIT License. The
following license terms apply to all files in the project:

  Permission is hereby granted, free of charge, to any person
  obtaining a copy of this software and associated documentation files
  (the "Software"), to deal in the Software without restriction,
  including without limitation the rights to use, copy, modify, merge,
  publish, distribute, sublicense, and/or sell copies of the Software,
  and to permit persons to whom the Software is furnished to do so,
  subject to the following conditions:

  The above copyright notice and this permission notice shall be
  included in all copies or substantial portions of the Software.

  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
  EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
  NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
  BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
  ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
  CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.

Contact
-------

This project is provided as-is, with no official support from
VMware. However, I will try to answer questions as time permits.
If you have questions or you'd like to submit a patch, feel free
to email me at: micah at vmware.com

--
