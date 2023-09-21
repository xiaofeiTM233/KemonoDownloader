# KemonoDownloader
Kemono下载工具

## 功能
下载Kemono上发布的图片，暂时不支持下载图片
下载的文件会按照每个投稿一个文件夹的形式存储在下载程序同路径下一个以作者用户名命名的文件夹下，同时保存介绍文本到ReadMe.txt中。

## 特别说明
本软件暂时仅支持GB2312(GBK)编码的Windows系统(即中文版Windows系统)，在其他语言版本下可能出现乱码和无法创建和读取文件等错误

## Special instructions
**This software only supports Windows systems with GB2312 (GBK) encoding (ie Chinese version of Windows system) for the time being. There may be garbled characters and errors such as unable to create and read files in other language versions
I am very sorry about this, maybe I will make it fit all versions of Windows in the future.**

## 使用方法
1. 下载Release中的KemonoDownloader.exe
2. 运行KemonoDownloader.exe
3. 选择代理方式
    3.1 如果你能够直连Kemono，输入'n'选择不使用代理，否则直接回车保持默认即可
    3.2 如果您选择了使用代理，请输入您的代理地址。请注意，本软件只支持Http代理。
        如果您的代理软件运行在本机，直接回车保持默认即可。
        如果您使用旁路由器或者其他设备作为代理，请输入代理设备的地址，例如'192.168.3.3',在这一步无需输入端口号，也不用添加http协议标识。
    3.3 输入代理IP以后，请输入代理端口号。如果您使用V2ray，这一步默认为V2ray的默认Http代理端口10809，直接回车确认即可。如果您的代理软件使用其他端口，请输入您的代理端口号并回车确认。
    3.4 如果您的代理需要用户名和密码，本软件不支持带用户名密码的代理，您可以考虑使用其他软件将代理转换为不带用户名密码的代理。
    3.5 确认代理无误后，请确认是否使用仅图片下载模式。该模式下将只会下载图片，且所有图片均存储在同一目录下。
    3.6 最后输入您要下载的作者的主页地址，例如 'https://kemono.su/patreon/user/1234567' ，然后回车确认。
        请注意，如果您在浏览作者主页时翻页过，那么请注意在粘贴地址时注意删去翻页参数"?o=0"，例如 'https://kemono.su/patreon/user/1234567?o=0' ，这样的地址是无法被本软件识别的，会导致作者主页无法被正常识别，在今后的版本中这个问题可能会被修复，但是现在请注意这一点。
    3.7 程序将会自动下载作者主页上的所有投稿，下载完成后会自动退出。
4. 如果您想要下载某位作者的特定某一期投稿，您可以选择运行KemonoDownloader_Single.exe，其使用方法与标准版大体相似，只要在填写下载地址时填入具体某篇投稿的地址即可，例如 'https://kemono.su/patreon/user/1234567/post/7654321' 。
    另外您还需要提供作者名称创建目录，这一步唯一的目的是创建目录，并不需要作者名称一定正确

## 注意事项
1. 本软件仅供学习交流使用，严禁用于商业用途
2. 本软件只提供了下载图像和说明的功能，暂时不支持下载作者提供的其他文件，如配套的视频、文本文档和压缩包等
3. 本软件不会对下载的文件进行任何修改，如果您下载的文件中包含有病毒或者其他恶意程序，本软件不承担任何责任
4. 本软件不会对您的任何行为进行监控，也不会收集您的任何信息

## ToDo
1. 合并标准版和Single版（也许会，但是再加一个选项是否太多了？）
2. 尝试支持其他语言版本的Windows系统（我暂时不知道怎么做，也没有相关的测试环境）
**2.E I'll try to support other language versions of Windows systems (I don't know how to do it for the time being, and I don't have a test environment)**
3. 提供对其他文件的下载支持
4. 适配Linux系统
5. 使用配置文件的方式来配置代理，以及其他参数
6. 提供一个GUI界面

## 使用的开源项目
本软件使用了LibCurl作为下载工具，本软件使用的是Windows下的自编译版本
