# [Vercel 汉化插件][project-url]

> 本项目源自: [qq sec/汉化vercel](https://greasyfork.org/zh-CN/scripts/473850-汉化vercel) [maboloshi/github-chinese](https://github.com/maboloshi/github-chinese)

  [![GitHub issues][issues-image]][issues-url]
  [![GitHub stars][stars-image]][stars-url]
  [![GitHub forks][forks-image]][forks-url]
  [![GreasyFork installs][greasyFork-image]][greasyFork-url]



## 🚩 功能

- 汉化 Vercel 页面，按钮等公共组件



## 🌐 浏览器与脚本管理器

浏览器                               | 脚本管理器
:----------------------------------: | :---------:
基于 Chromium 内核的PC浏览器 | [Tampermonkey][Tampermonkey] 或 [Violentmonkey][Violentmonkey]
Safari 浏览器（macOS, iOS, iPadOS）  | [Macaque][Macaque] 或 [Stay][Stay]
Firefox 或 基于 Gecko 内核的浏览器   | [Tampermonkey][Tampermonkey] 或 [Violentmonkey][Violentmonkey]
Via 浏览器（Android）                | 浏览器内置 
Kiwi 浏览器（Android） | [Tampermonkey][Tampermonkey] 



## 💽 安装

1. 请先安装用户脚本管理器。
1. 点击链接之一，安装脚本即可。
    - [GitHub 中文化插件 - GitHub 托管【开发版】（相对及时更新）][main.user.js]
        > 注意: 
        > 1. 当版本号未更新的情况下, 即使内容已更新, 用户脚本管理器依然会忽略, 需要手动安装获取更新
        > 2. 目前, 已实现每周一凌晨自动更新开发版版本号
    - [GitHub 中文化插件 - GreasyFork 托管【发布版】（仅大版本更新）][main(greasyfork).user.js]
1. 刷新下页面，即可发现网站已中文化。
> 需要视频教程的可以去看看[这里](https://github.com/maboloshi/github-chinese/discussions/133)收录的一些视频

> [!Note]
>
> ### 关于 “Chrome 127 及更高版本无法使用” 的问题
> 原因是 Chrome 127 及更高版本，陆续切换到 Manifest V3，目前已知 [Tampermonkey][Tampermonkey] 5.2.0 及以上版本支持，详见 [#234](https://github.com/maboloshi/github-chinese/issues/234) 讨论
> #### 解决方案：
> 1. 必须安装 [Tampermonkey][Tampermonkey] 5.2.0 及以上版本，其他脚本管理器暂不支持
> 2. 必须在浏览器的 “扩展程序” 管理中开启 “开发者模式”

## 词库本地调试方法
1. 需要安装用户脚本管理器 [Tampermonkey][Tampermonkey]，其他可能不支持。
1. 在浏览器扩展管理中，开启 [Tampermonkey][Tampermonkey] 的 “允许访问文件网址” 如图：

    <picture>
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/maboloshi/github-chinese/gh-pages/preview/允许访问文件网址-light.png"/>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/maboloshi/github-chinese/gh-pages/preview/允许访问文件网址-dark.png"/>
      <img src="https://raw.githubusercontent.com/maboloshi/github-chinese/gh-pages/preview/允许访问文件网址-light.png" width="75%" />
    </picture>

1. 将修改的词库文件放到方便访问的本地位置。
1. 安装 [GitHub 中文化插件 - GitHub 托管【开发版】（相对及时更新）][main.user.js]，实际 [GitHub 中文化插件 - GreasyFork 托管【发布版】（仅大版本更新）][main(greasyfork).user.js] 也可。
1. 回到脚本管理器，修改词库文件路径，即类似 `// @require      https://raw.githubusercontent.com/maboloshi/github-chinese/gh-pages/locals.js?v1.9.0`
   中网址改成本地路径格式如 `file:///D:/APP/github%E9%A1%B9%E7%9B%AE/github-chinese/locals.js`。

  > [!TIP]
  > 直接将词库文件拖到浏览器的地址栏，再复制地址栏的中地址即可。



## ✔ 待办 (TODO)

1. 添加 GitHub 名词解释，新手可能不太理解部分名词具体表达的意思，比如 `pull request`。
2. 整理部分 [Git](https://git-scm.com/) & [GitHub](https://github.com/) 学习资料, 帮助新手**更快**上手。



## ✨ 贡献



</details>

[project-url]: https://github.com/maboloshi/github-chinese "GitHub 中文化插件"

[issues-url]: https://github.com/maboloshi/github-chinese/issues "议题"
[issues-image]: https://img.shields.io/github/issues/maboloshi/github-chinese?style=flat-square&logo=github&label=Issue

[stars-url]: https://github.com/maboloshi/github-chinese/stargazers "星标"
[stars-image]: https://img.shields.io/github/stars/maboloshi/github-chinese?style=flat-square&logo=github&label=Star

[forks-url]: https://github.com/maboloshi/github-chinese/network "复刻"
[forks-image]: https://img.shields.io/github/forks/maboloshi/github-chinese?style=flat-square&logo=github&label=Fork

[license-url]: https://opensource.org/licenses/GPL-3.0  "许可证"
[license-image]: https://img.shields.io/github/license/maboloshi/github-chinese?style=flat-square&logo=github&label=License

[greasyFork-url]: https://greasyfork.org/scripts/435208  "GreasyFork - GitHub 中文化插件"
[greasyFork-image]: https://img.shields.io/badge/dynamic/json?style=flat-square&label=GreasyFork&query=total_installs&suffix=%20installs&url=https://greasyfork.org/scripts/435208.json

[Tampermonkey]: http://tampermonkey.net/ "篡改猴"
[Violentmonkey]: https://violentmonkey.github.io/ "暴力猴"
[Macaque]: https://macaque.app/ "猕猴"
[Stay]: https://apps.apple.com/cn/app/stay-for-safari-%E6%B5%8F%E8%A7%88%E5%99%A8%E4%BC%B4%E4%BE%A3/id1591620171 "Stay"

[main.user.js]: https://github.com/maboloshi/github-chinese/raw/gh-pages/main.user.js "GitHub 中文化插件 - GitHub 托管"
[main(greasyfork).user.js]: https://greasyfork.org/scripts/435208-github-%E4%B8%AD%E6%96%87%E5%8C%96%E6%8F%92%E4%BB%B6/code/GitHub%20%E4%B8%AD%E6%96%87%E5%8C%96%E6%8F%92%E4%BB%B6.user.js "GitHub 中文化插件 - GreasyFork 托管"

## 💝 鸣谢

[maboloshi](https://github.com/maboloshi) - 项目作者

[wuyuncheng-26](https://github.com/wuyuncheng-26) - 项目协作者

[52cik](https://github.com/52cik) - 项目原作者

### 感谢所有贡献者

一如既往，感谢我们出色的贡献者❤️！

<!--AUTO_GENERATED_PLEASE_DONT_DELETE_IT-->
<a href="https://github.com/maboloshi" title="沙漠之子">
  <img src="https://avatars.githubusercontent.com/u/7850715?v=4" width="42;" alt="沙漠之子"/>
</a>
<a href="https://github.com/52cik" title="楼教主">
  <img src="https://avatars.githubusercontent.com/u/5033310?v=4" width="42;" alt="楼教主"/>
</a>
<a href="https://github.com/wuyuncheng-26" title="是小胖呀26">
  <img src="https://avatars.githubusercontent.com/u/122529705?v=4" width="42;" alt="是小胖呀26"/>
</a>
<a href="https://github.com/TC999" title="陈生杂物房">
  <img src="https://avatars.githubusercontent.com/u/88823709?v=4" width="42;" alt="陈生杂物房"/>
</a>
<a href="https://github.com/qznfbnj" title="其智乃反不能及">
  <img src="https://avatars.githubusercontent.com/u/100760086?v=4" width="42;" alt="其智乃反不能及"/>
</a>
<a href="https://github.com/pylover7" title="大叶子">
  <img src="https://avatars.githubusercontent.com/u/56282729?v=4" width="42;" alt="大叶子"/>
</a>
<a href="https://github.com/cat-kun" title="cat-kun">
  <img src="https://avatars.githubusercontent.com/u/8529528?v=4" width="42;" alt="cat-kun"/>
</a>
<a href="https://github.com/pecasha" title="Pecasha">
  <img src="https://avatars.githubusercontent.com/u/9607128?v=4" width="42;" alt="Pecasha"/>
</a>
<a href="https://github.com/buiawpkgew1" title="菾凴">
  <img src="https://avatars.githubusercontent.com/u/71136405?v=4" width="42;" alt="菾凴"/>
</a>
<a href="https://github.com/3DMXM" title="小莫">
  <img src="https://avatars.githubusercontent.com/u/28587093?v=4" width="42;" alt="小莫"/>
</a>
<a href="https://github.com/xuexb" title="前端小武">
  <img src="https://avatars.githubusercontent.com/u/3872051?v=4" width="42;" alt="前端小武"/>
</a>
<a href="https://github.com/wang4yu6peng13" title="wang4yu6peng13">
  <img src="https://avatars.githubusercontent.com/u/10207042?v=4" width="42;" alt="wang4yu6peng13"/>
</a>
<a href="https://github.com/pangshitong" title="pangshitong">
  <img src="https://avatars.githubusercontent.com/u/41714457?v=4" width="42;" alt="pangshitong"/>
</a>
<a href="https://github.com/daydaygo" title="dayday">
  <img src="https://avatars.githubusercontent.com/u/3986303?v=4" width="42;" alt="dayday"/>
</a>
<a href="https://github.com/heicks" title="create new ██████╗  ██╔══██╗ ██████╔╝ ██╔══██╗ ██████╔╝ ╚═════╝  　　██╗ 　  ██╗ 　　██║ 　  ██║ 　　██║  　 ██║ 　　██║  　 ██║ 　　╚█████╔╝  　　╚═════╝  ███████╗ ██╔════╝　 ██║████═╗　 ██║　   ██　║ ╚██████╔╝　 　╚══════╝">
  <img src="https://avatars.githubusercontent.com/u/12287943?v=4" width="42;" alt="create new ██████╗  ██╔══██╗ ██████╔╝ ██╔══██╗ ██████╔╝ ╚═════╝  　　██╗ 　  ██╗ 　　██║ 　  ██║ 　　██║  　 ██║ 　　██║  　 ██║ 　　╚█████╔╝  　　╚═════╝  ███████╗ ██╔════╝　 ██║████═╗　 ██║　   ██　║ ╚██████╔╝　 　╚══════╝"/>
</a>
<a href="https://github.com/KS-OTO" title="KS-OTO">
  <img src="https://avatars.githubusercontent.com/u/6616413?v=4" width="42;" alt="KS-OTO"/>
</a>
<a href="https://github.com/swsoyee" title="InfinityLoop">
  <img src="https://avatars.githubusercontent.com/u/20528423?v=4" width="42;" alt="InfinityLoop"/>
</a>
<a href="https://github.com/ImgBotApp" title="Imgbot">
  <img src="https://avatars.githubusercontent.com/u/31427850?v=4" width="42;" alt="Imgbot"/>
</a>
<a href="https://github.com/CN-traveler" title="CN-traveler">
  <img src="https://avatars.githubusercontent.com/u/55753029?v=4" width="42;" alt="CN-traveler"/>
</a>
<!--AUTO_GENERATED_PLEASE_DONT_DELETE_IT-END-->

贡献者列表，由 [GitHub Action](https://github.com/maboloshi/github-chinese/blob/gh-pages/.github/workflows/update_contributors_images.yml) 自动生成
