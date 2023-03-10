+ 该配置配套教程：[zweix的win机器开发机配置指南](https://github.com/zweix123/CS-notes/blob/master/Missing-Semester/WindowsConfigGuide.md#5%E5%91%BD%E4%BB%A4%E8%A1%8C)

+ 提供的配置：
    1. oh-my-posh的主题：主打简约效率风，魔改自官方主题`ys`
    2. PowerShell7的配置：引入oh-my-posh和一个美化`ls`输出的模块
    3. Windows Terminal的配置：
        + 打开位置、打开大小、打开模式、模式切换快捷键
            >F4显示窗口栏（当然您可以改掉这个设置）
        + 字体种类、字体大小、One Dark风配色方案
          + 配色来[自](https://github.com/joshdick/onedark.vim)，One Dark风中的灰色过暗，我调教过，另外红色在vim中比较突兀，同样调教过。
        
    4. win下vim的配置，主要指文件`~\_vimrc`和目录`.\vimfiles\`，内容包括设置、主题（One Dark）和插件
        >这里的灰色没有调教过
    
    + 改键脚本：将`Caps`键改为方向键右键来加速使用oh-my-posh的补全

+ 关于终端配色风格，如果喜欢One Dark下面提供其他主题：
  + [官网提供](https://learn.microsoft.com/zh-cn/windows/terminal/custom-terminal-gallery/custom-schemes)：包括Ubuntu配色
  + [catppuccin](https://github.com/catppuccin/catppuccin)：确实很好看，但是体感总觉得更“锐”

## 使用

0. 下载：
    ```bash
    git clone https://github.com/zweix123/posh-config.git
    cd posh-config
    ```
+ 备份：可能出现报错，不过没关系
    ```powershell
    .\backup.ps1
    ```

1. 替换原有配置：
    ```powershell
    .\install.ps1
    ```
+ 收集：如果您Fork本项目做出自己的定制，这个脚本可以方便您在本地调试后将配置全部收集会本项目目录下
    ```powershell
    .\collect.ps1
    ```
    + 关于vim的插件本项目没有直接备份，而且在install脚本中使用下载的命令，所以collect脚本不能收集这部分