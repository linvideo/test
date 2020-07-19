|      | <!DOCTYPE html>                                              |
| ---- | ------------------------------------------------------------ |
|      | <html>                                                       |
|      | <head itemprop="Article" itemscope itemtype="http://schema.org/Article"> |
|      | <meta charset="UTF-8">                                       |
|      | <meta data-n-head="true" name="viewport" content="width=device-width,initial-scale=1,user-scalable=0"> |
|      | <meta name="theme-color" content="#de698c">                  |
|      | <meta http="Cache-Control" content="no-transform">           |
|      | <meta name="format-detection" content="telephone=no">        |
|      | <meta name="applicable-device" content="pc">                 |
|      | <link rel="apple-touch-icon-precomposed" href="[//static.hdslb.com/mobile/img/512.png](https://static.hdslb.com/mobile/img/512.png)"> |
|      | <link rel="icon" type="image/vnd.microsoft.icon" href="[//www.bilibili.com/favicon.ico](https://www.bilibili.com/favicon.ico)"> |
|      | <link rel="apple-touch-icon" href="[//www.bilibili.com/favicon.ico](https://www.bilibili.com/favicon.ico)"> |
|      | <meta name="name" content="小白也能白嫖:jsDelivr+FFmpeg打造切片视频床"> |
|      | <meta itemprop="title" name="title" content="小白也能白嫖:jsDelivr+FFmpeg打造切片视频床"> |
|      | <meta itemprop="description" name="description" content="了解jsd（jsdelivr）的小伙伴们通常都用它来当个图床用。但是，好不容易能薅资本主义的羊毛，白嫖党怎能就此罢休？下面就来解锁jsDelivr的高级玩法吧。jsDelivr实现切片视频播放个人博客使用Dplayer播放[你的名字]如上图，视频成品链接为https:&amp;#47;&amp;#47;cdn.jsdelivr.net&amp;#47;gh&amp;#47;huxx16&amp;#47;m3u8&amp;#47;yourname&amp;#47;playlist.m3u8嵌入Dplayer即可在个人博客内自建电影院。本文将讲述实现原理、介绍什么是m3u8、如何转码并切片视频以及上传使"> |
|      | <meta itemprop="keywords" name="keywords" content="FFMPEG,个人博客,格式工厂,音频处理,软件包,视频编码,AAC,MP4,GITHUB,老蘑菇,Your.Name,WINDOWS,linux,CMD,HTTPS,COPY,WIN,资本主义,你的名字,苹果公司,乱七八糟,老司机,小伙伴们,好不容易,视频网站,操作系统,莫名其妙,电影院,服务器,客户端,流畅度,同一个,2018年,HTTP,"> |
|      | <meta itemprop="author" name="author" content="王友元同学">  |
|      | <meta itemprop="url" content="https://www.bilibili.com/read/cv6103017/"> |
|      | <meta itemprop="image" content="https://i0.hdslb.com/bfs/article/9b87698a9e10a148d7853cd4c9627b941200fe9d.jpg"> |
|      | <meta itemprop="uploadDate" content="2020-5-17 21:41:50">    |
|      | <meta itemprop="datePublished" content="2020-5-17 21:41:50"> |
|      | <meta data-n-head="true" data-hid="og:type" property="og:type" content="article"> |
|      | <meta data-n-head="true" data-hid="og:title" property="og:title" content="小白也能白嫖:jsDelivr+FFmpeg打造切片视频床"> |
|      | <meta data-n-head="true" data-hid="og:image" property="og:image" content="https://i0.hdslb.com/bfs/article/9b87698a9e10a148d7853cd4c9627b941200fe9d.jpg"> |
|      | <meta data-n-head="true" data-hid="og:url" property="og:url" content="http://www.bilibili.com/read/cv6103017/"> |
|      | <meta name="renderer" content="webkit">                      |
|      | <meta name="spm_prefix" content="333.341">                   |
|      | <link data-n-head="true" rel="icon" type="image/x-icon" href="[//www.bilibili.com/favicon.ico](https://www.bilibili.com/favicon.ico)"> |
|      | <link data-n-head="true" rel="apple-touch-icon-precomposed" type="image/x-icon" href="http://static.hdslb.com/mobile/img/512.png"> |
|      | <link rel="Canonical" href="https://www.bilibili.com/read/cv6103017/"> |
|      | <link rel="stylesheet" type="text/css" href="[//static.hdslb.com/phoenix/dist/css/comment.min.css](https://static.hdslb.com/phoenix/dist/css/comment.min.css)"> |
|      | <title>小白也能白嫖:jsDelivr+FFmpeg打造切片视频床 - 哔哩哔哩</title> |
|      |                                                              |
|      | <script type="application/ld+json">                          |
|      | {                                                            |
|      | "@context": "http://schema.org/",                            |
|      | "@type": "Article",                                          |
|      | "@id": "https://www.bilibili.com/read/cv6103017/",           |
|      | "appid": "1580859622074471",                                 |
|      | "title": "小白也能白嫖:jsDelivr+FFmpeg打造切片视频床",       |
|      | "images": "https://i0.hdslb.com/bfs/article/9b87698a9e10a148d7853cd4c9627b941200fe9d.jpg", |
|      | "thumbnailUrl":"https://i0.hdslb.com/bfs/article/9b87698a9e10a148d7853cd4c9627b941200fe9d.jpg", |
|      | "description": "了解jsd（jsdelivr）的小伙伴们通常都用它来当个图床用。但是，好不容易能薅资本主义的羊毛，白嫖党怎能就此罢休？下面就来解锁jsDelivr的高级玩法吧。jsDelivr实现切片视频播放个人博客使用Dplayer播放[你的名字]如上图，视频成品链接为https:&amp;#47;&amp;#47;cdn.jsdelivr.net&amp;#47;gh&amp;#47;huxx16&amp;#47;m3u8&amp;#47;yourname&amp;#47;playlist.m3u8嵌入Dplayer即可在个人博客内自建电影院。本文将讲述实现原理、介绍什么是m3u8、如何转码并切片视频以及上传使", |
|      | "pubDate": "2020-5-17 21:41:50"                              |
|      | }                                                            |
|      | </script>                                                    |
|      | <script>                                                     |
|      | window.original = {                                          |
|      | cvid: "6103017",                                             |
|      | author: {                                                    |
|      | name: "王友元同学",                                          |
|      | mid: "516130979"                                             |
|      | },                                                           |
|      | banner_url: "",                                              |
|      | reprint: "0",                                                |
|      | summary: "了解jsd（jsdelivr）的小伙伴们通常都用它来当个图床用。但是，好不容易能薅资本主义的羊毛，白嫖党怎能就此罢休？下面就来解锁jsDelivr的高级玩法吧。jsDelivr实现切片视频播放个人博客使用Dplayer播放[你的名字]如上图，视频成品链接为https:&amp;#47;&amp;#47;cdn.jsdelivr.net&amp;#47;gh&amp;#47;huxx16&amp;#47;m3u8&amp;#47;yourname&amp;#47;playlist.m3u8嵌入Dplayer即可在个人博客内自建电影院。本文将讲述实现原理、介绍什么是m3u8、如何转码并切片视频以及上传使", |
|      | media: "",                                                   |
|      | actId: "0",                                                  |
|      | dispute: {                                                   |
|      | dispute: "",                                                 |
|      | dispute_url: ""                                              |
|      | },                                                           |
|      | spoiler: "0"                                                 |
|      | }                                                            |
|      | </script>                                                    |
|      | <link href="[//s1.hdslb.com/bfs/static/jinkela/article/pcDetail.0781a17edebcd4ac0c429f95d16ba720e050c593.css](https://s1.hdslb.com/bfs/static/jinkela/article/pcDetail.0781a17edebcd4ac0c429f95d16ba720e050c593.css)" rel="stylesheet"/></head> |
|      | <body>                                                       |
|      | <div id="biliMainHeader" class="report-wrap-module" style="height: 56px;"></div> |
|      | <div class="page-container">                                 |
|      | <div class="nav-tab-bar">                                    |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/home?from=articleDetail](https://www.bilibili.com/read/home?from=articleDetail)" target="_self" class="logo"> |
|      | </a>                                                         |
|      | <a href="[//www.bilibili.com/read/home?from=articleDetail](https://www.bilibili.com/read/home?from=articleDetail)" target="_self" class="tab-item" data-tab-id="0"> |
|      | <span>推荐</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/douga?from=articleDetail](https://www.bilibili.com/read/douga?from=articleDetail)" target="_self" class="tab-item " data-tab-id="2"> |
|      | <span>动画</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/game?from=articleDetail](https://www.bilibili.com/read/game?from=articleDetail)" target="_self" class="tab-item " data-tab-id="1"> |
|      | <span>游戏</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/cinephile?from=articleDetail](https://www.bilibili.com/read/cinephile?from=articleDetail)" target="_self" class="tab-item " data-tab-id="28"> |
|      | <span>影视</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/life?from=articleDetail](https://www.bilibili.com/read/life?from=articleDetail)" target="_self" class="tab-item " data-tab-id="3"> |
|      | <span>生活</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/interest?from=articleDetail](https://www.bilibili.com/read/interest?from=articleDetail)" target="_self" class="tab-item " data-tab-id="29"> |
|      | <span>兴趣</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/lightnovel?from=articleDetail](https://www.bilibili.com/read/lightnovel?from=articleDetail)" target="_self" class="tab-item " data-tab-id="16"> |
|      | <span>轻小说</span>                                          |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | <a href="[//www.bilibili.com/read/technology?from=articleDetail](https://www.bilibili.com/read/technology?from=articleDetail)" target="_self" class="tab-item  on" data-tab-id="17"> |
|      | <span>科技</span>                                            |
|      | </a>                                                         |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | </div>                                                       |
|      | <div class="up-info-holder">                                 |
|      | <div class="fixed-box">                                      |
|      | <div class="up-info-block">                                  |
|      | <a class="up-face-holder " href="[//space.bilibili.com/516130979](https://space.bilibili.com/516130979)" target="_blank"> |
|      | <img class="up-face-image" data-face-src="//i2.hdslb.com/bfs/face/561125b132f6c7639b6d0d8b5c74de151133cfe1.jpg" src="[//static.hdslb.com/images/member/noface.gif](https://static.hdslb.com/images/member/noface.gif)"> |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | </a>                                                         |
|      | <div class="up-info-right-block">                            |
|      | <div class="row">                                            |
|      | <a class="up-name" href="[//space.bilibili.com/516130979](https://space.bilibili.com/516130979)" target="_blank">王友元同学</a> |
|      | <span class="level"></span>                                  |
|      | <div class="nameplate-holder">                               |
|      | <i class="nameplate"></i>                                    |
|      | </div>                                                       |
|      | </div>                                                       |
|      | <div class="row-2">                                          |
|      | 粉丝:                                                        |
|      | <span class="fans-num"></span>                               |
|      | <span class="view">阅读:</span>                              |
|      | <span class="view-num"></span>                               |
|      | </div>                                                       |
|      | </div>                                                       |
|      | </div>                                                       |
|      | <div class="follow-btn-holder  ">                            |
|      | <span class="follow-btn">关注</span>                         |
|      | </div>                                                       |
|      | <div class="up-article-list-block hidden">                   |
|      | <div class="block-title">                                    |
|      | 推荐文章                                                     |
|      | </div>                                                       |
|      | <ul class="article-list">                                    |
|      | </ul>                                                        |
|      | </div>                                                       |
|      | <div class="more">                                           |
|      | <div class="top-bar">                                        |
|      | <label>更多</label>                                          |
|      | </div>                                                       |
|      | <a class="ac-link" href="[//www.bilibili.com/read/apply/](https://www.bilibili.com/read/apply/)" target="_blank"> |
|      | <div class="link">                                           |
|      | <span class="icon">                                          |
|      | </span>                                                      |
|      | <p class="title">成为创作者</p>                              |
|      | <p class="info">申请成为专栏UP主</p>                         |
|      | </div>                                                       |
|      | </a>                                                         |
|      | <a href="[//www.bilibili.com/blackboard/help.html#专栏相关](https://www.bilibili.com/blackboard/help.html#专栏相关)" target="_blank"> |
|      | <div class="help">                                           |
|      | <span class="icon">                                          |
|      | </span>                                                      |
|      | <p class="title">专栏帮助</p>                                |
|      | <p class="info">查看专栏使用说明</p>                         |
|      | </div>                                                       |
|      | </a>                                                         |
|      | </div>                                                       |
|      | </div>                                                       |
|      | </div>                                                       |
|      | <div class="right-side-bar">                                 |
|      | <div class="to-comment">                                     |
|      | <div class="comment-num-holder">                             |
|      | <span class="comment-num"></span>                            |
|      | </div>                                                       |
|      | </div>                                                       |
|      | <div class="to-top"></div>                                   |
|      | </div>                                                       |
|      | <div class="head-container">                                 |
|      |                                                              |
|      |                                                              |
|      | <div class="bangumi-rating-container"></div>                 |
|      |                                                              |
|      | <div class="argue-flag hidden"></div>                        |
|      | <div class="title-container">                                |
|      | <h1 class="title">小白也能白嫖:jsDelivr+FFmpeg打造切片视频床</h1> |
|      | <div class="info">                                           |
|      | <a class="category-link" href="[//www.bilibili.com/read/technology#rid=26](https://www.bilibili.com/read/technology#rid=26)" target="_blank"><span>数码</span></a> |
|      | <span class="create-time" data-ts="1589722918"></span>       |
|      | <div class="article-data"></div>                             |
|      | </div>                                                       |
|      | </div>                                                       |
|      |                                                              |
|      |                                                              |
|      | <div style="display:none" class="author-container">          |
|      | <a class="author-face" href="[//space.bilibili.com/516130979](https://space.bilibili.com/516130979)" target="_blank"> |
|      | <img data-face-src="//i2.hdslb.com/bfs/face/561125b132f6c7639b6d0d8b5c74de151133cfe1.jpg" src="[//i2.hdslb.com/bfs/face/561125b132f6c7639b6d0d8b5c74de151133cfe1.jpg](https://i2.hdslb.com/bfs/face/561125b132f6c7639b6d0d8b5c74de151133cfe1.jpg)" class="author-face-img"> |
|      |                                                              |
|      |                                                              |
|      |                                                              |
|      | </a>                                                         |
|      | <a class="author-name" href="[//space.bilibili.com/516130979](https://space.bilibili.com/516130979)" target="_blank">王友元同学</a> |
|      | <div class="attention-btn slim-border">关注</div>            |
|      | </div>                                                       |
|      | </div>                                                       |
|      |                                                              |
|      | <div class="article-holder"><p>  了解jsd（jsdelivr）的小伙伴们通常都用它来当个图床用。但是，好不容易能薅资本主义的羊毛，<span style="text-decoration: line-through;">白嫖党</span>怎能就此罢休？下面就来解锁jsDelivr的高级玩法吧。</p><h1><span class="font-size-23"><br/></span></h1><h1><span class="font-size-23">jsDelivr实现切片视频播放</span></h1><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/091d1950e1e7bc328d8bd14016eb7a7a09ab7e54.jpg" width="1171" height="656" data-size="57985"/><figcaption class="caption" contenteditable="">个人博客使用Dplayer播放[你的名字]</figcaption></figure><p>如上图，视频成品链接为https://cdn.jsdelivr.net/gh/huxx16/m3u8/yourname/playlist.m3u8</p><p>嵌入Dplayer即可在个人博客内自建电影院。</p><p>本文将讲述实现原理、介绍什么是m3u8、如何转码并切片视频以及上传使用。</p><p><span class="font-size-23"></span></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/4adb9255ada5b97061e610b682b8636764fe50ed.png" class="cut-off-5"/></figure><br/><h1><span class="font-size-23">如何实现</span><br/></h1><p>jsd能加载GitHub中单个20M以下的静态资源，所以能实现图床的功能。视频床也就是同样的道理，但通常视频的大小都超出了20M的大小限制。这时我们就可以<span class="color-pink-03">将视频切片，用m3u8索引 整合播放。</span></p><h1><span class="color-default font-size-23"><br/></span></h1><h1><span class="color-default font-size-23">m3u8是什么</span><br/></h1><blockquote><p><br/></p><p>m3u8是苹果公司推出的视频播放标准，是m3u的一种，只是编码格式采用的是UTF-8。</p><p>　　<strong><span class="color-pink-03">m3u8准确来说是一种索引文件，使用m3u8文件实际上是通过它来解析对应的放在服务器上的视频网络地址，从而实现在线播放。</span></strong>使用m3u8格式文件主要因为可以实现多码率视频的适配，视频网站可以根据用户的网络带宽情况，自动为客户端匹配一个合适的码率文件进行播放，从而保证视频的流畅度。</p></blockquote><p><span class="color-default font-size-16">将m3u8索引文件与视频切片放在GitHub同一目录下，即可通过jsd调用达到播放目的</span></p><p><span class="color-default font-size-23"><span class="font-size-16"><br/></span></span></p><p><span class="color-default font-size-23"><span class="font-size-16">jsDelivr与GitHub都明白，那标题里的FFmpeg又是什么？</span></span></p><p><span class="color-pink-02 font-size-20">FFmpeg是一套Linux环境下开发出来的视频音频处理程序，但它可以在包括 Windows 在内的大多数操作系统中编译。我们用它来将视频切片。</span></p><p><br/></p><p>手头有视频吗，现在就开始切片试试吧！</p><h1><span class="font-size-23">使用FFmpeg切片视频</span></h1><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/4adb9255ada5b97061e610b682b8636764fe50ed.png" class="cut-off-5"/></figure><h1><span class="font-size-23"></span></h1><p style="text-align: center;"><span class="color-default"><span class="color-default font-size-20">视频转码</span><br/></span></p><p><span class="color-pink-03"><span class="color-default">1.</span>对视频进行转码(转为 mp4)，将视频文件转为视频编码 h.264，音频编码 aac 格式的 mp4</span> <span class="color-pink-03">文件</span>，mp4 视频文件不是 h.264 编码到后面切片的时候可能会遇到很多莫名其妙的问题。</p><p><span class="color-pink-03">Q：如何转码？ </span></p><p><span class="color-pink-03">A：小白建议格式工厂</span>，老司机直接ffmpeg转吧，这里不提供ffmpeg转码教程了。格式工厂操作如下图<br/></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/956be5c182eb0e7f7a5dcab2f26ba2e30ae3d717.png" width="1150" height="500" data-size="79153"/><figcaption class="caption" contenteditable="">选择输出为MP4</figcaption><figcaption class="caption" contenteditable="">选择转出为MP4</figcaption></figure><p><span class="font-size-16"></span></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/5656c077441b011f4d4650c5c60d2f0fb8e67efe.png" width="947" height="611" data-size="43963"/><figcaption class="caption" contenteditable="">添加视频后，选择输出配置</figcaption></figure><p><br/></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/74c5c6dcc9bad43c3c4842047d4e031f6ca9763f.png" width="636" height="543" data-size="30424"/><figcaption class="caption" contenteditable="">如图设置完后，点击确定</figcaption></figure><p><span class="font-size-16"></span></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/1660099e76288650bdc11faf4a3fafc23eb38f0a.png" width="947" height="611" data-size="44020"/><figcaption class="caption" contenteditable="">再次确定</figcaption></figure><p><br/></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/434703a63527482215e08628357f78b0d0cebfbd.png" width="1150" height="500" data-size="86042"/><figcaption class="caption" contenteditable="">单机开始，然后等待完成</figcaption></figure><p>转码完成后输出MP4文件，我们记住它的位置</p><p><br/></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/4adb9255ada5b97061e610b682b8636764fe50ed.png" class="cut-off-5"/></figure><p style="text-align: center;"><span class="font-size-20">FFmpeg环境配置</span></p><p>2.去FFmpeg官网http://ffmpeg.org/下载软件包，软件包中找到主程序ffmpeg.exe<br/></p><p><br/></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/3ebaba1d82e01f0a43dbc746210bc386f1dfa03b.png" width="104" height="111" data-size="2298"/><figcaption class="caption" contenteditable="">没错就是它</figcaption></figure><p><span class="font-size-16"></span>我们将它复制</p><p><span class="font-size-16">粘贴到MP4的输出目录</span></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/3d8aa0f787089dcf372cb67a1fd061c07028856e.png" width="233" height="160" data-size="17849"/><figcaption class="caption" contenteditable="">放在一个目录中</figcaption></figure><p>win+R打开cmd，cd到这个目录</p><p>键入ffmpeg、回车。测试一下环境</p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/bcc482c49e548465cffaa876e0add6a4f68a8deb.png" width="672" height="293" data-size="30135"/><figcaption class="caption" contenteditable="">如上</figcaption></figure><p>显示<span class="font-size-16">如上选项即环境配置成功！</span></p><p><span class="font-size-20"><br/></span></p><h1><span class="font-size-20">开始切片，假设你的视频文件名为abd.mp4</span><br/></h1><p> 1.先用ffmpeg把<span class="color-pink-03">abc.mp4</span>文件转换为<span class="color-pink-03">abc.ts</span>文件：<span class="font-size-20"></span></p><p><span class="font-size-12">ffmpeg -y -i <span class="color-pink-03">abc.mp4</span> -vcodec copy -acodec copy -vbsf h264_mp4toannexb <span class="color-pink-03">abc.ts</span></span></p><p><br/></p><p> 2.再用ffmpeg把abc.ts文件切片并生成<span class="color-pink-03">playlist.m3u8</span>文件，5秒一个切片：</p><p><span class="font-size-12">ffmpeg -i abc.ts -c copy -map 0 -f segment -segment_list <span class="color-pink-03">playlist.m3u8</span> -segment_time <span class="color-blue-02 font-size-12">5</span> <span class="color-pink-03">abc%03d.ts</span></span></p><p><span class="color-default font-size-16">这其中<span class="color-blue-02 font-size-16">5<span class="color-default font-size-16">表示5秒一个切片，可以自行更改（<span class="color-pink-03 font-size-16">单个大小要在20m以下</span>）</span></span><br/></span></p><p><span class="color-pink-03 font-size-16"><span class="color-default font-size-16">(</span> playlist.m3u8可以自行改成xxx.m3u8 ，如更改则最终组成链接时需要对应的更改文件名<span class="color-default font-size-16">)</span></span></p><p><span class="color-default font-size-16"><span class="color-blue-02 font-size-16"><span class="color-default font-size-16"><span class="color-default font-size-16">等待完成，我们得到<br/></span></span></span></span></p><p><span class="color-default font-size-16"><span class="color-blue-02 font-size-16"><span class="color-default font-size-16"><span class="color-default font-size-16"></span></span></span></span></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/4ec3fd2176ae4d609bffeea6a747c99a8a8a2d8c.png" width="842" height="345" data-size="44853"/><figcaption class="caption" contenteditable="">如图</figcaption></figure><p> 和</p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/4df4e0d6696d08b1c65f26f3bcc0dbf675b96f5a.png" width="575" height="335" data-size="53656"/><figcaption class="caption" contenteditable="">如图</figcaption></figure><p>说明切片成功！（<span class="color-pink-03">切片失败的原因可能是你磁盘空间不足导致</span>）<span class="color-default font-size-16"></span><br/></p><h1><span class="font-size-20"><br/></span></h1><h1><span class="font-size-20">上传所有文件至GitHub</span><br/></h1><p><span class="font-size-16">这就不用解释了吧。。<span class="color-pink-03 font-size-16">上传m3u8文件以及所有的xxx.ts文件</span></span><br/></p><p><span class="font-size-16">记得放在同一个文件目录中！</span></p><p><span class="font-size-16">最终完成和我们的视频链接为</span></p><p>https://cdn.jsdelive.net/gh/GitHub用户名/库名/文件目录/<span class="color-pink-03">playlist.m3u8</span></p><p><span class="color-pink-03"><br/></span></p><p><span class="color-pink-03"><span class="color-default">Eg：如图用户huxx16,文件存放在名为&#34;m3u8&#34;的库下/yourname目录</span></span></p><figure class="img-box" contenteditable="false"><img data-src="//i0.hdslb.com/bfs/article/c773be0210b5cc46c0682215312934ee47464223.png" width="1035" height="476" data-size="46480"/><figcaption class="caption" contenteditable=""></figcaption></figure><p>对应的链接就为 <span class="color-pink-03"><span class="color-default">https://cdn.jsdelivr.net/gh/huxx16/m3u8/yourname/playlist.m3u8</span></span></p><p><span class="color-default"><span class="color-default font-size-23">以上！</span><br/></span></p><p><span class="color-default"><span class="color-default font-size-23"><br/></span></span></p><p><span class="font-size-16">什么？你说m3u8怎么播放？百度找个解析接口套进去试试吧</span></p><p>以上乱七八糟的教程早在2018年就有人在CSDN上提出了理论。我也有参考老蘑菇https://m1314.cn/403.html的这篇文章。可能我唯一做到的就是讲的乱七八糟了亿点吧。</p><p>个人博客https://moetuan.cn/，欢迎各位大佬前来拜访！</p><p><span class="color-pink-03"><br/></span><br/></p><p><span class="color-pink-03"><span class="color-default"></span><br/></span><br/></p><p><span class="font-size-20"><br/></span><br/></p><p><span class="color-default font-size-20"><br/></span><br/></p><p><span class="color-default font-size-23"><br/></span></p></div> |
|      |                                                              |
|      |                                                              |
|      | <p class="authority">本文禁止转载或摘编</p>                  |
|      |                                                              |
|      |                                                              |
|      | <div class="article-action">                                 |
|      | <div class="ops">                                            |
|      | <span class="like-btn">                                      |
|      | <i class="icon-video-details_like"></i>                      |
|      | <span>--</span>                                              |
|      | </span>                                                      |
|      | <span class="coin-btn">                                      |
|      | <i class="icon-video-details_throw-coin"></i>                |
|      | <span>--</span>                                              |
|      | </span>                                                      |
|      | <span class="fav-btn">                                       |
|      | <i class="icon-video-details_collection"></i>                |
|      | <span>--</span>                                              |
|      | </span>                                                      |
|      | <span class="share-container share-btn">                     |
|      | 分享到：<span></span>                                        |
|      | </span>                                                      |
|      | </div>                                                       |
|      | <div class="more">                                           |
|      | <!-- <i class="icon-general_more-actions"></i> -->           |
|      | <div class="more-ops-list">                                  |
|      | <ul>                                                         |
|      | <li value="0">投诉或建议</li>                                |
|      | </ul>                                                        |
|      | </div>                                                       |
|      | </div>                                                       |
|      | </div>                                                       |
|      | <div class="article-list-holder-block"></div>                |
|      | <div class="draft-holder-block">                             |
|      | </div>                                                       |
|      | <div class="b-head comment-title-block">                     |
|      | <span class="b-head-t comment-results" style="display: inline;"></span> |
|      | <span class="b-head-t">评论</span>                           |
|      | </div>                                                       |
|      | <div class="comment-holder"></div>                           |
|      |                                                              |
|      | </div>                                                       |
|      | <div id="biliMainFooter" class="report-wrap-module"></div>   |
|      | <script src="[//static.hdslb.com/public/intersection-observer.js](https://static.hdslb.com/public/intersection-observer.js)"></script> |
|      | <script src="[//static.hdslb.com/public/timing.min.js](https://static.hdslb.com/public/timing.min.js)"></script> |
|      | <script>window.performanceLog.setSource('article');</script> |
|      | <script src="[//static.hdslb.com/js/jquery-3.3.1.min.js](https://static.hdslb.com/js/jquery-3.3.1.min.js)"></script> |
|      | <script>                                                     |
|      | window.reportMsgObj = {}                                     |
|      | window.reportConfig = {                                      |
|      | sample : 1,                                                  |
|      | errorTracker : false ,                                       |
|      | resourceTracker: false ,                                     |
|      | scrollTracker: false,                                        |
|      | msgObjects : 'reportMsgObj'                                  |
|      | }                                                            |
|      | </script>                                                    |
|      | <script type="text/javascript" charset="utf-8" src="[//s1.hdslb.com/bfs/seed/jinkela/header-v2/header.js](https://s1.hdslb.com/bfs/seed/jinkela/header-v2/header.js)"></script> |
|      | <script type="text/javascript" src="[//s1.hdslb.com/bfs/seed/jinkela/footer-v2/footer.js](https://s1.hdslb.com/bfs/seed/jinkela/footer-v2/footer.js)"></script> |
|      | <script src="[//s1.hdslb.com/bfs/seed/jinkela/short/config/biliconfig.js](https://s1.hdslb.com/bfs/seed/jinkela/short/config/biliconfig.js)"></script> |
|      | <script type="text/javascript" src="[//static.hdslb.com/phoenix/dist/js/comment.min.js](https://static.hdslb.com/phoenix/dist/js/comment.min.js)"></script> |
|      | <script src="[//s1.hdslb.com/bfs/static/biliapp/biliapp.js](https://s1.hdslb.com/bfs/static/biliapp/biliapp.js)"></script> |
|      | <!-- <script type="text/javascript" src="//s1.hdslb.com/bfs/seed/log/report/log-reporter.js" crossorigin></script> --> |
|      | <script>                                                     |
|      | (function(){                                                 |
|      | var src = (document.location.protocol == "http:") ? "http://js.passport.qihucdn.com/11.0.1.js?e6352779c080ceddc1bc4c6bbe047b69":"https://jspassport.ssl.qhimg.com/11.0.1.js?e6352779c080ceddc1bc4c6bbe047b69"; |
|      | document.write('<script src="' + src + '" id="sozz"><\/script>'); |
|      | })();                                                        |
|      | </script>                                                    |
|      | <script type="text/javascript" src="[//s1.hdslb.com/bfs/static/jinkela/article/manifest.0781a17edebcd4ac0c429f95d16ba720e050c593.js](https://s1.hdslb.com/bfs/static/jinkela/article/manifest.0781a17edebcd4ac0c429f95d16ba720e050c593.js)"></script><script type="text/javascript" src="[//s1.hdslb.com/bfs/static/jinkela/article/vendor.0781a17edebcd4ac0c429f95d16ba720e050c593.js](https://s1.hdslb.com/bfs/static/jinkela/article/vendor.0781a17edebcd4ac0c429f95d16ba720e050c593.js)"></script><script type="text/javascript" src="[//s1.hdslb.com/bfs/static/jinkela/article/pcDetail.0781a17edebcd4ac0c429f95d16ba720e050c593.js](https://s1.hdslb.com/bfs/static/jinkela/article/pcDetail.0781a17edebcd4ac0c429f95d16ba720e050c593.js)"></script></body> |
|      | </html>                                                      |
|      |                                                              |
