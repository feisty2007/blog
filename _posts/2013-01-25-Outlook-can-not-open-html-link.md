---
layout: tb1
title: Outlook 2007无法打开链接"由于本机的限制 该操作已被取消"
---

## {{ page.title}}
原因：安装过chrome，firefox或其它第三方浏览器导致outlook无法打开链接。

 

如果你尝试过

重设IE；

设置默认程序；

WORD Internet链接设置；

均无效。或者，

轻信了那些

“你的系统中毒了”

“重装系统吧”

之类的“后现代脑残型答案”后，还没有解决问题的话，往下看。

 
运行-》regedit-》

找到 HKEY_CURRENT_USER/Software/Classes/.html 
右边默认值更改为：htmlfile

依次类推 .htm .shtml .xhtm .xhtml

打开outlook，点击email里的链接，IE窗口跳出来。

搞定。

{{ page.date | date_to_string }}