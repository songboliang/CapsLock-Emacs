# CapsLock-Emacs

借助AHK实现CapsLock+的功能，主要借鉴了了Emacs的光标移动和复用了Ctrl的部分功能

> 感谢Feng Ruohang的脚本，感谢开源的AHK软件  
> [AHK官网][AHK官网]  
> [Feng Ruohang的原脚本网址][Feng Ruohang的原脚本网址]  

## 描述:

  基于Feng Ruohang的脚本编写的适配Emacs方向按键设定的脚本,精简了部分内容，修改了部分内容，增加了部分内容。

主要为两个部分：

- 添加Emacs风格的光标移动，基于CapsLock实现。CapsLock + pnbf 来冗余（重复）上下左右的功能，CapsLock + ae来冗余Home、End功能键，到达行首行尾
- 冗余Ctrl的功能。CapsLock + zxcv Space tab 等去冗余对应的Ctrl+的功能，其中CapsLock+v使用了Ditto，来实现历史粘贴的功能。

借助与AHK可以在不破坏原有快捷键的基础上增添一个CapsLock为功能键，本脚本提供CapsLock+系列的拓展映射，让你更专注的进行编辑(光标移动)，释放你的小拇指(替代Ctrl)     

##概览:        

| 快捷键           | 描述                                                         |
| ---------------- | ------------------------------------------------------------ |
| CapsLock;        | {ESC}  发送退出命令                                          |
| CaspLock + u     | {CapsLock} 取代原本的CapsLock的功能                          |
| CapsLock + pnbf  | Emacs-Style的光标移动，p是previous向上，n是next，b是back光标向后，f是forward光标向前。 |
| CapsLock + ae    | a是{Home},跳到行首，e是{End}，跳到行尾。                     |
| CapsLock + d     | {Delete} 删除键                                              |
| CapsLock + zxcv  | 冗余原本的Ctrl + zxcv 其中CapsLock + v实际使用的是Ditto的功能，可以调用剪贴板，查看历史粘贴 |
| CapsLock + Space | Ctrl + Space 切换输入法                                      |
| Alt + CapsLock   | Alt + Ctrl 标签切换之类的功能                                |

[AHK官网]: https://autohotkey.com/
[Feng Ruohang的原脚本网址]: https://github.com/Vonng/Capslock/blob/master/win/CapsLock.ahk