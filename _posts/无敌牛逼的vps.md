---
title: 无敌牛逼的vps
abbrlink: 49631
date: 2022-07-22 08:37:14
tags:
categories: 技术
---
无敌牛逼的vps
# 无敌牛逼的vps
前几个月一直在想vps的问题，在想有了一台vps之后我可以在上面干点什么，有趣的是结果当我真有了vps后却不知道怎么办了
那么今天就在这里水一篇博文，主要是这台vps真的很良心，首先要说明的是**完全免费**，真的太香了！！
**有root访问权限，Debian系统，x86架构要比ibm的更实用些，4核32G而且部署还简单，无需信用卡！！**
梦中情机属于是😂
***但是！注意！免费的午餐是没有的！！请不要搭建完就跑，一定要看服务条款，文章最后我会截取最重要的那部分给大家，一定要看服务条款！一定要看服务条款！一定要看服务条款！***
那么就开始申请吧！
<!-- more -->
# 劝退二连
首先有个注册超30天的GitHub账号，其次这个帐号绑定的邮箱不能是qq/163以及国内主流邮箱，建议gamil或在中国能方便注册的hotmail，我就是用hotmail成功的。
# 注册流程
一、打开页面：https://github.com/MetaVPS/xssh 直接登录，Fork这个仓库，库名称一定要保持xssh；

二、打开页面：https://dashboard.ngrok.com/login 直接使用GitHub账号登录，然后在入门-授权令牌/Getting Started-Your AuthToken 里找到```Copy```，直接复制

三、在你自己仓库中修改config.sh,内容为 NGROK_TOKEN="你的令牌"，然后返回仓库，拷贝仓库地址，格式例如：https://github.com/你的名字/xssh

四、打开页面：https://cloud.okteto.com/#/login 同样用GitHub登录。**注意：这一步如果用国内邮箱会显示该GitHub账号的邮箱不符合规范**然后在左上角点击：新建开发环境-GitUrl。填写上一个步骤中你的仓库的地址（*https://github.com/你的名字/xssh*)，分支填写 main，然后启动。稍等1-3分钟，直到网络部署显示Running！

五、我们回到ngrok，在左侧栏里找到Tunnels- Agent，然后点击里面的栏目，会弹出来类似tcp://6.tcp.ngrok.io:12795 这样的一个地址。

这样就可以了，接下来我们进行ssh连接，你的用户名和密码和我保持一致，地址和端口要看你自己的后台哦：
地址：6.tcp.ngrok.io端口：12795用户名：root密码：majalaya

***很重要的是，一定一定要看他的服务条款，接下来我截取一些重要的，我因为搭建MInecraft服务器而被封了一个号，同时搭建代理也是不允许的！！！***

# 服务条款
> ## 禁止的内容
通过您的应用程序或使用我们服务的其他网站显示和/或处理的内容不包含以下任何类型的内容：
1.根据适用法律侵犯第三方权利（例如版权）的内容。
2.过于亵渎的内容。
3.与仇恨相关或暴力内容。
4.旨在倡导或推进计算机黑客攻击或破解的内容。
5.赌博。
6.非法活动，包括但不限于非法出口受管制物质或非法软件。
***7.网络钓鱼。***
***8.恶意内容。***
9.违反或鼓励违反任何刑法、任何其他适用法律或任何第三方权利的行为的其他材料、产品或服务。
> ## 禁止的行为
此外，您不得也不得允许任何第三方，包括您的最终用户：
1.生成、分发、发布或便利未经请求的群发电子邮件、促销、广告或其他招标（“垃圾邮件”）。
2.故意分发病毒、蠕虫、缺陷、特洛伊木马、损坏的文件、恶作剧或任何其他破坏性或欺骗性的物品。
3.冒充他人（通过使用电子邮件地址或其他方式）或以其他方式歪曲自己或任何电子邮件的来源。
4.无需Okteto事先书面批准，即可创建自动化帐户或批量注册帐户。
5.使用我们的服务侵犯他人的合法权利（如隐私权和公开权）。
6.促进或鼓励非法活动。
7.干扰其他用户对我们服务的享受。
***8.执行负载测试。***
9.出售、交易或转售对我们服务的访问权限。
10.修改、改编、翻译或逆向工程我们服务的任何部分。
11.使用我们的服务进行点对点文件共享。
***12.使用我们的服务“开采”加密货币或比特币。***
***13.使用我们的服务运行“Minecraft”或类似的服务器。***
***14.使用我们的服务运行Telegram和WhatsApp机器人或类似服务。***
***15.使用自动化服务来规避我们服务中的限制和配额，例如帐户共享、批量帐户创建或自动请求调度。***
***16.使用我们的服务操作“开放代理”或任何其他形式的互联网代理服务，能够将请求转发给任何最终用户或第三方提供的互联网主机。***(就是搭建梯子！！！)
17.使用我们的服务或与我们的服务提供的任何接口，以违反使用此类Okteto产品或服务的条款或其他条款和条件的方式访问任何Okteto产品或服务。

# 最后的话
说实话，免费的午餐果然没有，这个服务器限制还是稍微有些多的，这也是为什么我拿到vps之后迷茫了，不知道干什么，原本计划好的事全部都被禁止了，但是这个服务器应该还可以用来建站。下篇文章我会写一个专门用于搭建MInecraft服务器的免费vps，配置还不错，就这样。