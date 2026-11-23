---
title: "Windows 用户的命令行母语：5 类场景、7 个命令、4 步让 AI 替你写"
source: "https://workbuddy.jiangyufan.com/index/hub/case/1001"
type: "case"
chars: 2337
sections: 7
figures: 3
chapter: "10-我要写代码和做自动化"
---

# Windows 用户的命令行母语：5 类场景、7 个命令、4 步让 AI 替你写
## 为什么 Windows 用户也需要命令行
很多人对 Windows 的印象还停留在「点点鼠标」的年代。但企业 IT 运维、数据批量处理、自动化任务，这些场景 PowerShell 才是最专业的工具。

**一个真实场景：**批量给 1000 个文件重命名。用鼠标，右键、重命名、输入新名、按 Tab、下一个，至少点 1000 次，半小时没了。用 PowerShell，一行命令，10 秒搞定。

**结论：**PowerShell 不是「装 X 工具」，是 Windows 上处理重复任务的效率倍增器。

![左边点击 10 次菜单，右边一行命令，效率差 10 倍](https://workbuddy.jiangyufan.com/uploads/attach/2026/11/20261121/f4e77dacc111b4657ed9f9bfb71fc83b.png)

*左边点击 10 次菜单，右边一行命令，效率差 10 倍*

![Get-ChildItem 加 Rename-Item 一行命令完成批量重命名](https://workbuddy.jiangyufan.com/uploads/attach/2026/11/20261121/f5f4a36ff4b2c50e7a5ab0e66ff4f688.png)

*Get-ChildItem 加 Rename-Item 一行命令完成批量重命名*

## 和 Bash 的区别
上一期讲了 Bash 是 Linux/Mac 的命令行工具。PowerShell 类似 Bash，但有几个关键不同。

运行平台：Bash 在 Linux、macOS；PowerShell 在 Windows，也可以装在 Mac 和 Linux。输出类型：Bash 输出纯文本，PowerShell 输出对象，可以直接管道传给下一个命令做二次处理。命令风格：Bash 简短（ls、cd、cp），PowerShell 是动词-名词（Get-ChildItem、Set-Location）。默认安装：Win10/11 都已预装 PowerShell 5.1 和 PowerShell 7。

**结论：**如果你只用 Windows，PowerShell 就是你的命令行母语，比 Bash 更直观。

## 五个最实用的场景
场景一，批量文件操作，1 小时变 1 分钟。把 D 盘所有 .txt 文件后缀改成 .md，一条 Get-ChildItem 加 Rename-Item 就够。

场景二，系统信息查询，不用装任何工具。一键查看电脑全部硬件信息：Get-ComputerInfo 配合 Select-Object 取 Windows 版本、处理器、物理内存。

场景三，批量装卸软件，IT 运维神器。静默安装用 Start-Process msiexec.exe 加 /quiet 参数；批量卸载用 Get-Package 筛名字再管道到 Uninstall-Package。

场景四，日志分析，出问题时救命。查最近 1 小时系统错误日志：Get-EventLog -LogName System -EntryType Error -After (Get-Date).AddHours(-1)。

场景五，网络诊断，程序员和运维必备。查本机所有网络连接用 Get-NetTCPConnection 筛 Established 状态；测试到百度的连接用 Test-NetConnection 指定 443 端口。

![AI 大脑联动多个 PowerShell 终端，覆盖各种管理任务](https://workbuddy.jiangyufan.com/uploads/attach/2026/11/20261121/a8ca7401634f9b1d45752ac460fea455.png)

*AI 大脑联动多个 PowerShell 终端，覆盖各种管理任务*

## Windows 用户必会的 7 个命令
Get-ChildItem，看当前目录，简写 ls 或 dir，加 -Recurse 递归查所有文件。

Set-Location，切目录，等同于 cd。切到 D 盘写 Set-Location D:\，回上级写 Set-Location ..，回根目录写 Set-Location \。

Copy-Item 和 Move-Item，复制和移动。复制整个文件夹要加 -Recurse。

Remove-Item，删除，慎用。删文件夹含子文件要 -Recurse -Force，加 -Force 就不进回收站了，务必想清楚。

Get-Content，读文件，等同于 cat。加 -Wait 可以实时跟踪日志。

Get-Process 和 Stop-Process，管进程。查占用 CPU 最高的 5 个进程：Get-Process 按 CPU 降序取前 5；强杀进程用 Stop-Process 加 -Force。

Get-Help，自带字典，不会就问它。查任何命令的用法：Get-Help Get-Process -Examples。

## 4 步让 AI 直接帮你写命令
你不需要记住所有命令，让 AI 帮你写。这是 WorkBuddy 最核心的玩法。

第一步，用自然语言告诉它你想要什么。比如「帮我写一条 PowerShell 命令：把 D:\photos 目录下所有大于 10MB 的 jpg 文件压缩到 50% 画质，输出到 E:\backup\photos」。它会输出可直接运行的脚本。

第二步，先在小范围测试，这步很重要。加 -WhatIf 参数模拟运行，不实际执行，只显示会发生什么。

第三步，确认无误后正式执行，去掉 -WhatIf 直接跑就行。

第四步，第一次执行时打开回收站，或者先备份重要数据。命令行的删除不进回收站，这一步是最后的保险。

## 5 个常见翻车实录
删错文件，因为没加过滤条件。教训：删除前必须先 ls 看清楚，永远加 -WhatIf 先模拟。

权限不足，因为没以管理员身份运行。教训：操作 C 盘、系统文件夹、安装软件，必须右键「以管理员身份运行」PowerShell。

中文路径乱码，编码问题。PowerShell 7 默认 UTF-8，5.1 是 GBK。脚本开头加一行设置输出编码为 UTF-8。

执行策略被禁止，脚本无法运行。系统默认禁止运行 .ps1 脚本，先用 Set-ExecutionPolicy RemoteSigned 放开。

误关系统进程，电脑黑屏。教训：别手贱 Stop-Process 名字含 svchost、csrss、lsass 的进程，会直接蓝屏。

## 写在最后
读完这篇，你应该明白三件事：PowerShell 是 Windows 原生的高效工具；五类场景分别是文件、系统、软件、日志、网络；七个必会命令是 Get-ChildItem、Set-Location、Copy-Item、Remove-Item、Get-Content、Get-Process、Get-Help。

鼠标能做的事，PowerShell 做得更快；鼠标做不了的事，PowerShell 做得到。
