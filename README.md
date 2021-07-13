# 基于易语言的Minecraft客户端半自动更新<br>

## 关于项目

<font size=4><strong>uzuki chii(羽月ちい)  MC客户端定制自动更新</font></strong>

<font size=5 color=red><strong>占位，尚未发布</font></strong>

<font size=4><strong>羽月ちい：[twitter](https://twitter.com/uzukichii) / [bilibili](https://live.bilibili.com/22870039) / [youtube](https://www.youtube.com/channel/UCJxPldVojkxP1lQZuPskJtg)</font></strong>

## 使用环境

<font size=4><strong>仅支持windows</font></strong>

## 使用须知

非盈利开源软件 仅保留除支持库外的原创内容著作权 可二次修改 如果可以 请尽量在修改后的软件中署名原作者osttsStudio<br><br>
<s>因为易语言的原因 下载之前先关掉360和电脑管家之类的东西 defender防止报毒的方法：退出360和电脑管家 然后在安全中心里[添加排除项](https://jingyan.baidu.com/article/b87fe19e22f8435219356840.html)</s><br><br>
通过增加加密壳的方式防止误报 目前测试defender会报毒但不会删文件 微软smartscreen会拦截 360和电脑管家没反应 Edge会报毒阻止下载 解决方法暂时未知<br><br>
关于二次开发的问题 服务器参数文件可以按照源码对照编写 因为涉及到下载url的问题 暂时不提供 之后可能会写一份通用版的文件（划重点 可能）

## 关于功能

通过判断版本号 启动时检测是否有更新，如果没有直接运行启动器，不运行窗体，如果有更新，点击按钮自动下载解压覆盖，覆盖以后会用新版本客户端替换掉自身并运行启动器

## 如何编译

### 二次开发

调用的支持库：HTTP进度下载类/精易模块/超级模块<br><br>
编译（所有文件注入exe）：易语言读取.e文件->编译->静态编译

#### 关于封包

Themida或其他封包软件

### 直接使用

从releases下载（并不一定会提供最新版本，可下载老版本自动更新）

## 如何使用

将启动器改名为client.exe，可自定义更新程序的名字，同时需要修改bat文件<br>

运行更新程序，检测到新版本时会自动显示窗体，点击start，程序会自动完成，之后就是正常启动游戏的步骤（自己的服务器请下载源码修改url然后重构）

## 更新日志

- 2021.07.14 当config.ini不存在时会重新下载程序 需要手动确认
- 2021.07.14 当client.exe不存在时会提示报错
- 2021.07.14 程序识别当前版本改为读取本地配置文件
- 2021.07.05 标题从服务器获取改为固定 相关自定义修改 包括但不限于文件名 下载路径
- 2021.06.17 修复了当没有更新直接运行启动器时程序获取路径错误的bug
- 2021.06.16 通过bat文件替换自身