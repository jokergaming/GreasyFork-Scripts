# [**GreasyFork-Scripts**](https://f9y4ng.github.io/GreasyFork-Scripts/) - F9y4ng -  [![WIKI](https://img.shields.io/badge/WIKI-GREASYFORK%20SCRIPTS-brightgreen.svg?logo=github "wiki")](https://github.com/F9y4ng/GreasyFork-Scripts/wiki)

[![LICENSE](https://img.shields.io/badge/License-GPL--3.0--only-blue.svg?style=for-the-badge&logo=github "LICENSE")](https://github.com/F9y4ng/GreasyFork-Scripts/blob/master/LICENSE)
[![LAST COMMIT](https://img.shields.io/github/last-commit/F9y4ng/GreasyFork-Scripts?color=blue&logo=github&style=for-the-badge "LAST COMMIT")](https://github.com/F9y4ng/GreasyFork-Scripts/commits/master)
[![ISSUES](https://img.shields.io/github/issues/F9y4ng/GreasyFork-Scripts?logo=github&style=for-the-badge "ISSUES")](https://github.com/F9y4ng/GreasyFork-Scripts/issues)
[![STARS](https://img.shields.io/github/stars/F9y4ng/GreasyFork-Scripts?color=brightgreen&logo=github&style=for-the-badge "STARS")](https://github.com/login?return_to=%2FF9y4ng%2FGreasyFork-Scripts)

请先根据你的浏览器安装一个**用户脚本管理器**扩展(如TamperMonkey, ViolentMonkey) 然后再**安装脚本**。

(不建议使用AdGuard安装脚本，因为脚本设置功能将无法查看。如有配置需要，请使用“键盘快捷键”。)

***

## 字体渲染（自用脚本）[**Font Rendering.user.js**](https://github.com/F9y4ng/GreasyFork-Scripts/blob/master/Font%20Rendering.user.js)

简介：无需安装MacType，优化浏览器字体显示，让每个页面的中文字体变得有质感，默认使用微软雅黑字体，亦可自定义设置多种中文字体，附加字体描边、字体重写、字体阴影、字体平滑、对特殊样式元素的过滤和许可等效果，脚本菜单中可使用设置界面进行参数设置，亦可对某域名下所有页面进行排除渲染，兼容常用的 Greasemonkey 脚本和浏览器插件。

> `version 2022.02.20.2`

`!!! 重大版本更新，请使用前仔细查看` [[脚本使用说明 - WIKI](https://github.com/F9y4ng/GreasyFork-Scripts/wiki/Font_Rendering)] `New !!!`

`!!! 首次使用前请仔细阅读使用说明！仔细阅读使用说明！阅读使用说明 !!!`

`!!! 为保证您的数据安全，请及时备份您的本地数据！请勿使用来源未知的备份文件 !!!`

```text
+ 延长字体列表缓存时间至一周，提升页面启动速度。
@ 修正在Chromium V96.0及以上版本Blink内核浏览器下，对粗体样式描边渲染的bug，并优化代码执行性能。
@ 修正某些网站因远程字体载入超时，造成脚本菜单不显示，或造成字体表解析缓慢使配置页面样式错误的bug。
@ 修正Firefox的字体描边效果在选取文字时出现的渲染错误，并对明亮及黑暗模式优化渲染效果。
@ 修正其他小问题，优化CSS兼容性，优化代码。
```

### **关于问题反馈**

> 请反馈问题的朋友注意：反馈脚本错误或样式显示问题，请把**仅使用本脚本的情况下**发生问题的**具体访问网址**、使用的**浏览器版本**、**脚本运行器版**、**相关错误的截图**、以及**具体操作流程**或**错误提示**（如果有的话）发出来，你遇到的问题不一定能在其他地方复现。

* [关于个别网站样式错误修正的设置分享，不定期更新，自取自用。](https://github.com/F9y4ng/GreasyFork-Scripts/discussions/42)

* 字体表字体及其他中文字体分享：[点这里下载字体包](https://github.com/F9y4ng/GreasyFork-Scripts/discussions/46)

### **关于字体的添加**

> **如果您需要向字体表添加自定义字体，请按[帮助说明的指引](https://github.com/F9y4ng/GreasyFork-Scripts/wiki/Font_Rendering#customfont)进行操作。**

> 如果您需要增加新的字体进入代码字体表，请将 **完整且准确** 的字体 **中文全称** 及 **英文全称** 按 **预设格式** 添加进自定义字体列表。格式如：`{"ch":"鸿蒙黑体", "en":"HarmonyOS Sans SC"}`
>
> * 新增字体，一般只接受字重为 **标准体/Regular** 的字体，需调整字重粗体请使用字体描边进行设置。
> * 网络上很多字体存在各种修改版、Hack 版，非原版字体会造成字体名不一致，从而使得代码无法识别。

> 每当您的计算机安装了新字体，若要使其 **立即生效**，请在“ **高级核心功能设置** ”中为当前网站重建字体列表缓存。
> * 注1：由于操作系统字体缓存，在计算机安装新字体后请**重启浏览器**，确保系统字体缓存在浏览器中生效。
> * 注2：要使所有域名网站的字体列表均立刻生效，可进入浏览器设置清空所有缓存。（ctrl+shift+del）

### **关于字体缩放**

> 字体比例缩放（正式版），默认关闭，请在 **高级核心功能设置** 中打开字体缩放功能。
>
> * **已知问题：** 因Firefox的Gecko内核对JS及CSS限制，建议Firefox用户谨慎使用该功能。
> * **未知情况：** 如在非Firefox浏览器中遇到样式异常或坐标偏移，请及时向我[反馈](https://github.com/F9y4ng/GreasyFork-Scripts/issues)。

### **字体渲染（自用脚本）的新版本已完成，在使用新版脚本前，请注意以下事项：**

> 新版脚本中 **内置了默认的字体渲染样式，该样式为我本地配置，并不能完美适配于你的计算机**。所以，首次使用时，如果出现渲染效果没有达到理想状态，属于**正常情况**。请根据**自有显示器的配置及设置**，通过**脚本配置界面**修正相关参数来达到最佳显示效果。如在使用过程中遇到错误或使用问题，请及时向我[反馈](https://github.com/F9y4ng/GreasyFork-Scripts/issues)。

***

## 谷歌、百度、必应的搜索引擎跳转工具 [**Google & Baidu Switcher.user.js**](https://github.com/F9y4ng/GreasyFork-Scripts/blob/master/Google%20%26%20Baidu%20Switcher.user.js)

简介：最新版本的集合谷歌、百度、必应的搜索引擎跳转工具，必应跳转可在菜单进行自定义设置。此版本无外部脚本调用，更快速和准确的进行按钮定位，显示速度大大提升。如有异常请清空浏览器缓存，再次载入使用，感谢使用！

> `version 4.1.20220122.1`

`!!! 重大版本更新，请使用前仔细查看` [[脚本使用说明 - WIKI](https://github.com/F9y4ng/GreasyFork-Scripts/wiki/Google_Baidu_Switcher)] `New !!!`

`!!! 自动更新检测默认开启，如无更新提示需求，可在“功能设置开关”中关闭它 !!!`

```text
@ 优化RAF函数, 提高代码执行性能。
@ 修正一些bugs.
```

### **重要说明**

> 新版本“**自动更新**”功能默认开启，如不需要更新检测，请在脚本菜单“功能设置开关”中，关闭 **更新检测** 即可。
>
> * 请反馈问题的朋友注意：反馈脚本错误或样式显示问题，请把发生问题的**具体访问网址**、使用的**浏览器版本**、**脚本运行器版**、**相关错误的截图**（仅开本脚本的情况下的）、以及**具体操作流程**或**错误提示**（如果有的话）发出来，你遇到的问题不一定能在其他地方复现。
>
> * 一般来说，最新及测试版的发布将在**Github**进行，**GreasyFork**会在24小时内自动同步。已开启自动更新检测功能的用户，客户端代码会根据更新频率设置进行自动更新。
>
