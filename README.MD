七月音乐播放器
========
七月音乐播放器 是一款开源的基于 `Meting` 的在线音乐播放器。具有音乐搜索、播放、下载、歌词同步显示、个人网易云音乐播放列表同步等功能。

前端界面参照 QQ 音乐网页版进行布局，同时采用了流行的响应式设计，无论是在PC端还是在手机端，均能给您带来原生 app 般的使用体验。
### 注意事项
-----
#### 运行环境
php 5.4+, curl_exec, file_get_contents, json_decode, openssl_encrypt

#### 兼容性
本播放器设计支持 IE9及以上的现代浏览器。并且已在 Chrome、firefox、IE11 等浏览器测试使用正常。

### 更新日志
-----
#### v3.0 `2018/4/1`
- 更改初始化的列表为指定歌手
- 重构了DataApiDeal.php
- 其它一些细节优化

#### v2.41 `2018/3/13`
- 修复 IE 下播放键错位的 BUG
- 修改默认背景为黑色
- 其它一些细节优化

#### v2.4 `2018/3/11`
- 修复网易云音乐无法播放
- 增加标题栏滚动效果(感谢@lzcykevin)
- 增加歌曲循环播放控制(感谢@yuxizhe)
- 修复百度音乐无法播放
- 优化连续播放失败的歌曲过多时，自动终止播放。防止卡死
- 压缩图片素材，限制封面图片尺寸，优化页面加载速度
 

-----
#### 播放列表DIY教程
本播放器支持后台自定义播放列表。打开 `js/musicList.js`，按照里面的说明对应修改即可。

#### 播放器DIY教程
除了自定义播放列表，本播放器还支持一些 DIY 设定，比如修改 api.php 文件的默认路径、修改搜索框的默认搜索内容等。具体请打开 `js/player.js` 查看

#### rem 变量表
程序中的rem数组用于存储全局变量，具体的成员(部分)及作用见下表：

| 变量名    | 用途   |
| ----------- | ----------- |
| rem.audio | audio dom |
| rem.playlist | 当前正在播放的播放列表编号 |
| rem.playid | 正在播放的这首歌在播放列表中的编号 |
| rem.dislist | 当前显示的列表的列表编号 |
| rem.loadPage | 搜索功能已加载的页码 |
| rem.wd | 当前的搜索词 |
| rem.source | 当前选定的音乐源 |
| rem.uid | 当前已同步的用户的网易云 ID |
| rem.uname | 已登录用户的用户名 |
| rem.sheetList | 歌单容器操作对象 |
| rem.mainList | 歌曲列表容器操作对象 |
| rem.isMobile | 是否是手机浏览 |

### 致谢
 
#### 采用的开源模块
- **Jquery**：js主流开发框架 [http://jquery.com/](http://jquery.com/)
- **Meting**：一个高效的多平台音乐 API 框架 [https://github.com/metowolf/Meting](https://github.com/metowolf/Meting)
- **layer**：一款强大的web弹层组件 [http://layer.layui.com/](http://layer.layui.com/)
- **mCustomScrollbar**：jQuery自定义滚动条样式插件 [http://manos.malihu.gr/jquery-custom-content-scroller/](http://manos.malihu.gr/jquery-custom-content-scroller/)
- **background-blur**：跨浏览器磨砂效果背景图片模糊特效插件 [https://msurguy.github.io/background-blur/](https://msurguy.github.io/background-blur/)
- **Let's Kill IE6**：消灭IE [http://overtrue.me](http://overtrue.me)

##### 在开发过程中，还参照了很多开源 html 播放器的相关代码，在此一并向他们表示感谢！
##### 感谢VUE音乐客户端, 网易Github开源API等的帮助

### 版权
七月播放器,是在MK播放器的原有基础上进行了改造,
基于 [https://github.com/mengkunsoft/MKOnlineMusicPlayer](https://github.com/mengkunsoft/MKOnlineMusicPlayer),
感谢MK大牛[https://github.com/mengkunsoft](mengkun)的无私开源精神
### 劝告
`奉劝某些“人”保留住做人的最基本底线，遵守开源协议`
