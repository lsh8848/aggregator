<!--
 * @Author: wzdnzd
 * @Date: 2022-03-06 14:51:29
 * @Description: 
 * Copyright (c) 2022 by wzdnzd, All Rights Reserved.
-->

## 功能
打造免费代理池，爬一切可爬节点
> 拥有灵活的插件系统，如果目标网站特殊，现有功能未能覆盖，可针对性地通过插件实现

> 欢迎 Star 及 PR。对于质量较高且普适的爬取目标，亦可在 Issues 中列出，将在评估后选择性添加

## 使用方法
> 略，自行探索。我才不会告诉你入口是 `collect.py` 和 `process.py`。**强烈建议使用后者，前者只是个小玩具**，配置参考 `subscribe/config/config.default.json`

1，依次开启workflow，比如Collect,Process和Checkin

2，创建gist并获取到username/gist_id（记得保存，稍后要用），打开 https://gist.github.com ，随便创建一个，内容随便填

3，回到 Sign in to GitHub · GitHub ( https://github.com/settings/tokens?type=beta )，点击Generate new token按钮创建 PAT。名字随便填，过期时间选得久一点，重要的是在Account permissions里授予Gists的读写权限，创建好后复制生成的token稍后用

4，到仓库页面的Settings里设置环境变量，变量名为GIST_LINK和GIST_PAT，值分别为第4和5两步获取到的内容

5,启用Action后如果中途你不想搞了，一定要禁用workflow或Action，因为默认每两小时自动执行一次

## 免责申明
+ 本项目仅用作学习爬虫技术，请勿滥用，不要通过此工具做任何违法乱纪或有损国家利益之事
+ 禁止使用该项目进行任何盈利活动，对一切非法使用所产生的后果，本人概不负责
