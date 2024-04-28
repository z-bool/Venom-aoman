# Aoman去指纹浏览器 - 伪造一个安全的渗透环境

**郑重声明：文中所涉及的技术、思路和工具仅供以安全为目的的学习交流使用，<u>任何人不得将其用于非法用途以及盈利等目的，否则后果自行承担</u>** 。

>  此项目于阿呆安全团队-aoman编译

<small>此工具请于github下载，此处纯源码编译保证无毒，其他地方下载的不知道有无嵌入shellcode</small>

<p align="center"><a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-_red.svg"></a><a href="https://github.com/z-bool/Venom-aoman"><img  src="https://goreportcard.com/badge/github.com/projectdiscovery/httpx"></a></p>

<p align="center"><a href="#install">项目介绍</a> · <a href="#detail">使用详情</a> <a href="#communicate"> · <a href="#notice">注意事项</a> · <a href="#communicate">技术交流</a></p>

<div id="install"></div>
<h3>项目介绍</h3>

为何要重新编译Chromium浏览器，用一个去指纹浏览器有什么好处？

- 在爬虫逆向时候，可以通过刷新浏览器页或者新建浏览器标签页即得到全新的浏览器环境，可以帮助我们更快速更便捷的发现参数变化
- 在渗透测试时候，可以通过对浏览器环境的伪造绕过部分限制，配上插件和可变隧道就可以大大增加溯源的工作量。

编译去指纹浏览器修改了哪些指纹？

- Canvas
- Color
- Webgl
- Webgl2
- Render
- Vender
- Image_hash
- Webaudio
- WebRTC

<div id="detail"></div>
<h3>使用详情</h3>

![image-20240428125016030](https://github.com/z-bool/Venom-aoman/blob/main/1.png?raw=true)

浏览器指纹查看：https://browserleaks.com/canvas

正常指纹截图：
![image-20240428125843074](https://github.com/z-bool/Venom-aoman/blob/main/2.png?raw=true)

现在我们用去指纹浏览器查看一下：
![image-20240428130150750](https://github.com/z-bool/Venom-aoman/blob/main/3.png?raw=true)

开一个新标签：
![image-20240428130302468](https://github.com/z-bool/Venom-aoman/blob/main/4.png?raw=true)

<div id="notice"></div>

<h3>注意事项</h3>

- 请从https://github.com/z-bool/Venom-aoman直接下载纯净编译的chromium。
- 启动时跳powershell窗口，应该是最小打包哪个依赖没打进来吧，没加🐎，不放心的话自查一下

<div id="communicate"></div>

<h3>技术交流</h3>

<img src="https://cdn.jsdelivr.net/gh/z-bool/images@master/img/qrcode_for_gh_c90beef1e2e7_258.jpg" alt="阿呆攻防公众号" style="zoom:100%;" />
