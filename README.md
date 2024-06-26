# 私域引流宝

👋 私域引流宝致力于为个人、团队提供基于微信私域流量的推广、引流的效率工具。可减轻人力，有效降低资源损失、流量流失的几率。引流宝完全开源，免费，可商用、可任意二次开发。引流宝可以辅助你更好地开展营销活动推广！降低运营成本，提高工作效率，获取更多资源。
<br/><br/>
👉 群活码使用场景：<br/>
微信群二维码有效期是7天，7天后二维码过期无法扫码进群，或者是群人数满200人就无法扫码进群。如果在推广的时候，群满人或者过期了，别人还想进群，我们将会失去很多推广资源。所以有了 **`群活码`**，可在不更换链接和二维码的前提下，切换扫码后显示的内容，保证你推广出去的二维码或链接可以持续为你提供引流效果！<br/><br/>

👉 客服码使用场景：<br/>
当你的工作需要同时给不同的人对接客户数据，又要保证大家对接的频率、次数、效果保持平均，中途如果需要增加或者减少对接人，客服码就可以解决这个问题。客服码可以让一个人先对接你设置的人数，自动轮到下一个人对接，也就是阈值展示二维码，当你的二维码达到扫码最大值，就轮到下一个人的展示。当然也可以随机展示。<br/><br/>

👉 短网址使用场景：<br/>
生成的短网址可以控制其访问权限，例如仅限在微信内访问，或者不能在微信访问，或者仅限电脑浏览器访问，仅限安卓手机访问，仅限苹果手机访问。短链接在推广活动中，有着精简而不简单的作用，你还可以有完全控制权。<br/><br/>

![ylb](https://p0.meituan.net/dpmerchantpic/7c65fbbb4614748eedb6243b2649fde191004.jpg%40200w_200h_1e_1l)

# 更新日志
![](https://img.shields.io/badge/Version-2.4.3-brightgreen.svg)<br/>
1. 2.4.3版本新特性：<br>
2. UI界面大量的优化<br>
3. 新增群活码并流<br>
4. 新增短网址轮询域名<br>
5. 外部跳微信抽离出来作为插件<br>
6. 群活码、客服码、渠道码整合到活码一栏<br>
7. 提供用户账号注册<br>
8. 渠道码新增操作系统渠道数据记录<br>
9. 新增卡密分发小程序管理<br>
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
v2.4.3是基于v2.4.0修复了一些已知的小问题，具体如下：<br/>
1. 适配jumpWX插件的抖音云;（只需替换代码，无需执行升级程序）<br/>
2. 插件新增对非管理员使用权限的设置;（只需替换代码，无需执行升级程序）<br/>
3. 修复短链接无法启用群活码并流程序；(需手动创建数据库字段，具体请看bug修复日志）<br/>
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
**bug修复日志：** <br/><br/>
2024年6月3日，收到用户反馈，通过短链接访问的群活码，无法并流。经过排查是短链接的调度器没有对并流做处理，现已完成维护，如果你是 `2.4.0 - 2.4.2` 版本用户，你可以下载发生变动的代码替换到你服务器的代码，具体如下：<br/>
```
1. /s/index.php
2. /static/css/ylb.css
3. /console/qun/addBingliu.php
4. /console/qun/index.html
5. /console/qun/qun.js
6. 前往数据库 `ylb_qun_bingliu` 这个表手动添加一个 `before_qun_key` 字段 `[varchar(10)]`
```
* 全新安装以及旧版升级到 `2.4.3` 版本的，忽略这个提醒，请直接下载完整版进行安装和升级。

# 私域引流宝Pro

私域引流宝Pro正在开发中，该版本使用全新的技术栈，Vue3+Pinia+Javascript+Acro Design，专注于精细化多用户运营，敬请期待！

![](https://img10.360buyimg.com/imgzone/jfs/t1/195291/18/46886/46491/6671a08bFb39178b7/758ccfd004478483.jpg)

# 公众号
![](https://img10.360buyimg.com/imgzone/jfs/t1/145303/24/42799/5773/662f19e0Fe49e9666/ca57d11bc2c9de54.jpg)

# 全新安装

访问 install 目录即可进入安装流程。<br/>

示例：
```
http://域名/install/
```
安装成功后请删除 /install/ 目录。

# 版本升级

**升级步骤如下：** <br/>
1、升级前请备份好数据；<br/>
2、备份 console/Db.php 这个文件；<br/>
3、备份 console/upload/ 目录； <br/>
4、下载新版本代码；<br/>
5、将 console/Db.php 这个文件以及 console/upload/ 目录替换；<br/>
6、访问install目录，选择你要升级的版本选项。<br/>

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=likeyun/liKeYun_Ylb&type=Date)](https://star-history.com/#likeyun/liKeYun_Ylb&Date)

# 卡密分发小程序源码
请付费购买：https://afdian.net/item/270573e4f97d11eea18d5254001e7c00

# 使用文档
https://docs.qq.com/doc/DREdWVGJxeFFOSFhI <br/><br/>

就算你是个小白0基础，没有服务器、没有域名，不会搭建服务器，不会搭建网站，使用指南中有个针对0基础的教程，看完就会了。

# 开发程序语言
前端：Bootstrap+jQuery<br/>
后端：php+mySql

![](https://img.shields.io/badge/PHP-7.4.0-brightgreen.svg) ![](https://img.shields.io/badge/Bootstrap-4.0-brightgreen.svg) ![](https://img.shields.io/badge/jQuery-3.6.0-brightgreen.svg)

# 使用
管理后台路径：/console/index/<br/>

示例：
```
http://域名/console/index/
```

# 功能

![](https://img10.360buyimg.com/imgzone/jfs/t1/208894/5/41649/168432/661f99cdFe7276d89/a8ea2fc7db99aa40.png)

# 截图
![](https://img10.360buyimg.com/imgzone/jfs/t1/164167/30/43171/104800/661f9729Ff4dd4d0e/78ef16d0e86a6dc1.jpg)
![](https://img20.360buyimg.com/imgzone/jfs/t1/191563/24/44191/58534/661a9ddbF5cfc547c/17ad9f196524cf63.jpg)
![](https://img20.360buyimg.com/imgzone/jfs/t1/200610/12/41550/56663/661a9ddbFbd1bed37/c61186595872aa02.jpg)
![](https://img20.360buyimg.com/imgzone/jfs/t1/228263/40/15024/53748/661a9ddaF22c7697d/972690898e4532fa.jpg)
![](https://img20.360buyimg.com/imgzone/jfs/t1/105851/13/42644/64819/661a9ddeFb60a873a/93fce70b7cad5b1e.jpg?1713020502922)
![](https://img20.360buyimg.com/imgzone/jfs/t1/217676/11/40259/86985/661a9ddeFdd8a2702/a2a9823bcfa0106e.jpg?1713020511515)
![](https://img20.360buyimg.com/imgzone/jfs/t1/134110/23/41436/77328/661a9de0Fbfe14345/023b1bfc4cc4a872.jpg?1713020521891)
![](https://img20.360buyimg.com/imgzone/jfs/t1/234089/31/15393/69706/661a9ddfF29f026cd/a9cc2eb6038304dc.jpg?1713020536505)
![](https://img20.360buyimg.com/imgzone/jfs/t1/131277/30/41020/114973/661a9ddcF7f73a838/b4bad634ee39499d.jpg?1713020550421)

# 域名定时检测

免费开源版不带定时域名检测，这款的配置中心自带一个域名检测任务，你可以对指定的域名创建一个域名检测任务，通过宝塔面板的定时任务实现自动检测域名是否被微信拦截、封禁的情况，检测到被封可以收到通知。<br/><br/>
![](https://img10.360buyimg.com/imgzone/jfs/t1/195926/10/46451/89427/666027a6Fa155b77c/cb560f8a85240bb2.jpg)
![](https://img10.360buyimg.com/imgzone/jfs/t1/189615/4/45168/88627/666027a5F81d75fc4/c318b110eae48c37.jpg)

**私域引流宝2.4.3定制版 - 带域名检测任务模块购买链接：** https://afdian.net/item/9e620960231811efa2f65254001e7c00 <br/><br/>
购买后，你可以选择全新安装，也可以选择版本升级。如果你是基于 `2.3.0` 版本升级，需要查看使用文档中版本升级的方法完成升级，如果你是基于 `2.4.0` 版本。那么只需要替换代码（请备份 `Db.php` 和 `upload` 目录）后登录即可使用。

# 赞赏
赞赏作者，支持长期维护开源项目。<br/><br/>
<img src="http://p18.qhimg.com/t014667134b2634568a.jpg" width="400" />

**最近一个月赞赏记录**

| 用户昵称 | 赞赏渠道 | 赞赏金额 |
| ----- | ----- | ----- |
| 潜行 | 微信 | 20.00 |
| 小智 | 微信 | 88.00 |
| 青禾 | 微信 | 50.00 |
| MR、Guan | 微信 | 50.00 |
| Jason | 微信 | 16.00 |
| 不知名 | 微信 | 20.00 |
| Miro | 微信 | 20.00 |
| 马轩 | 微信 | 88.00 |
| 党老师 | 微信 | 50.00 |
| Soujer | 微信 | 188.00 |
| 长卿@奇人匠心 | 微信 | 16.80 |
| 有谱i | 微信 | 50.00 |
| 一米多一米 | 微信 | 20.00 |
| 维嘉 | 微信 | 20.00 |
| 技术老胡 | 微信 | 10.00 |
| Ikun🏀 | 微信 | 266.00 |
| 雨声好入眠 | 微信 | 10.00 |
| LinK | 微信 | 20.00 |
| 柳听风 | 微信 | 50.00 |
| LERO | 微信 | 50.00 |
| 小智 | 微信 | 88.00 |
| 侠狼¹主号 | 微信 | 10.00 |
| 小伟 | 微信 | 18.88 |
| wang | 微信 | 88.00 |
| 来到这个世界... | 微信 | 50.00 |
| 随性且随风 | 微信 | 18.80 |
| 肖荣铭 | 微信 | 20.00 |
| 李来信 | 微信 | 20.00 |
| 筱炯 | 微信 | 30.00 |

# 交流群
目前有7个交流群，以邀请方式加入<br/>
如需进群请添加群主微信号<br/>
微信号：sansure2016 <br/><br/>
<img src="http://p17.qhimg.com/t01c5795ee4423dba85.jpg" width="300" /><br/><br/>
微信群日常活跃，高质量，没有广告，欢迎各位网友加入。<br/>

# 作者
Name：TANKING<br/>
WeChat：sansure2016<br/>
Blog：https://segmentfault.com/u/tanking<br/>
From：Guangdong Canton<br/><br/>
<img src="http://p18.qhimg.com/t01fa8997c05a7243cd.jpg" width="200" />

# 旧版
1.3.0：https://likeyun.lanzout.com/i4doR0jhtw8b <br/>
2.0.0：https://likeyun.lanzout.com/imKAq143yfkd <br/>
2.1.0：https://likeyun.lanzout.com/iyh7l1gm5iyh <br/>
2.2.0：https://likeyun.lanzout.com/igRQG1iw53xi <br/>
2.3.0：https://likeyun.lanzout.com/iRwGW1uzuqtc <br/>

# 开源协议
![](https://img.shields.io/badge/开源协议-MIT-brightgreen.svg) 该软件遵循MIT开源协议。

# 提醒
该软件仅适用于辅助日常工作，提高工作效率，减轻人力。请勿用于诈骗、黑灰产业，如有此类行为，后果自负。
