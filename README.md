<div align="center">

[![python](https://img.shields.io/badge/python-3.7%2B-blue)](http://www.python.org/download)
[![PyPI](https://img.shields.io/pypi/v/biliup)](https://pypi.org/project/biliup)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/biliup)](https://pypi.org/project/biliup)
[![license](https://img.shields.io/github/license/biliup/biliup)](https://github.com/biliup/biliup/blob/master/LICENSE)
[![Telegram](https://img.shields.io/badge/Telegram-Group-blue.svg?logo=telegram)](https://t.me/+IkpIABHqy6U0ZTQ5)
</div>

  <h3 align="center">biliup</h3>

  <p align="center">
    录制各大主流直播并上传至哔哩哔哩弹幕网。
    
<br />
    <a href="https://biliup.github.io/biliup/docs/guide/changelog"><strong>更新日志 »</strong></a>
    <br />
    <br />
    <a href="https://github.com/biliup/biliup/wiki/%E5%AE%89%E8%A3%85-%E8%BF%90%E8%A1%8C-%E6%9B%B4%E6%96%B0-%E5%8D%B8%E8%BD%BD">简易教程</a>
    ·
    <a href="https://biliup.me/">交流社区</a>
    ·
    <a href="https://github.com/biliup/biliup-app">投稿工具</a>
  </p>
</div>

    

<details>
<summary>详细介绍</summary>

* 支持自动录制各大主流直播平台实时直播流，并于录制结束后自动上传到哔哩哔哩视频网站。
* 支持YouTube，twitch直播回放列表自动搬运至b站，如链接 https://www.twitch.tv/xxxx/videos?filter=archives&sort=time
* 支持录制哔哩哔哩，斗鱼，虎牙，Twitch平台的**直播弹幕**，生成B站标准格式的XML弹幕文件，可被常见的各种弹幕挂载程序使用处理
* 自动选择上传线路，保证国内外vps上传质量和速度
* 从 v0.4.32 版本开始，不依赖配置文件可直接使用webUI，若想和低于 v0.4.32 时一致使用配置文件，请添加启动参数`--no-http`
* 可分别控制下载与上传并发量
* ~~支持 cos-internal，腾讯云上海内网上传，免流 + 大幅提速~~
* 实验性功能：
    - 防止录制花屏（使用默认的stream-gears下载器就会有这个功能）

</details>

**社区教程**： [图文教程](https://www.bilibili.com/read/cv33195912) by [@ikun1993](https://github.com/ikun1993)编写。


## Quick Start

1. `pip3 install biliup`
2. `biliup start`
3. 启动时访问 `http://your-ip:19159` 使用webUI，
****

![](.github/resource/light.png)
![](.github/resource/dark.png)

## How to Contribute
1. nodejs `version >= 18`
2. `npm i`
3. `npm run dev`
4. `python3 -m biliup`
5. 访问`http://localhost:3000`
****
## 支持

| 直播平台 | 支持类型      | 链接示例 | 特殊注释 |
| :------:| :------: | ------ | ------ |
| 虎牙 | 直播 | `https://www.huya.com/123456` | 可录制弹幕 |
| 斗鱼 | 直播 | `https://www.douyu.com/123456` | 可录制弹幕 |
| YY语音 | 直播 | `https://www.yy.com/123456` |
| 哔哩哔哩 | 直播 | `https://live.bilibili.com/123456` | 特殊分区hls流需要单独配置/可录制弹幕 |
| acfun | 直播 | `https://live.acfun.cn/live/123456` |
| afreecaTV | 直播 | `https://play.afreecatv.com/biliup123/123456` | 录制部分直播时需要登陆 |
| bigo | 直播 | `https://www.bigo.tv/123456` |
| 抖音 | 直播 | 直播:`https://live.douyin.com/123456`<br>主页:`https://www.douyin.com/user/456789(抖音号)` | 录制douyin.com/user/类型链接或被风控需配置cookies |
| 快手 | 直播 | `https://live.kuaishou.com/u/biliup123` |
| 网易CC | 直播 | `https://cc.163.com/123456` |
| flextv | 直播 | `https://www.flextv.co.kr/channels/123456/live` |
| 映客 | 直播 | `https://www.inke.cn/liveroom/index.html?uid=123456` |
| 猫耳FM | 直播 | `https://fm.missevan.com/live/123456` | 猫耳为纯音频流 |
| nico | 直播 | `https://live.nicovideo.jp/watch/lv123456` | 可配置登录信息 |
| twitch | 直播/回放 | 直播:`https://www.twitch.tv/biliup123`<br>回放:`https://www.twitch.tv/biliup123/videos?filter=archives&sort=time`  | 可配置登录信息/尽量录制回放/可录制弹幕 |
| youtube | 直播/回放 | 直播:`https://www.youtube.com/watch?v=biliup123`<br>回放:`https://www.youtube.com/@biliup123/videos` | 可配置登录信息/尽量录制回放/可配置回放下载日期 |
* 理论上streamlink与yt-dlp支持的都可以下载，但不保证可以正常使用，详见:[streamlink支持列表](https://streamlink.github.io/plugins.html)，[yt-dlp支持列表](https://github.com/yt-dlp/yt-dlp/tree/master/yt_dlp/extractor).
****

## Credits
* Thanks `ykdl, youtube-dl, streamlink` provides downloader.
* Thanks `THMonster/danmaku`.
****

## 捐赠
* 维护一个开源项目并不是个简单的事，那么，请作者喝杯咖啡吧~૮(˶ᵔ ᵕ ᵔ˶)ა
* 爱发电 :`https://afdian.net/a/biliup`
****



## Stars
[![Star History Chart](https://api.star-history.com/svg?repos=biliup/biliup&type=Date)](https://star-history.com/#biliup/biliup&Date)
