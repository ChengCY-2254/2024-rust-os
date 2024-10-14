## 参考资料
<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=459886905&bvid=BV1Q5411w7z5&cid=319792271&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
## 寄存器
#寄存器
RISC-V寄存器编号从`0-31`，表示为`x0-x31`。其中: `x10-x17`对应`a0-a7`。`x1`对应`ra`
约定的寄存器`a0-a6`保存系统调用的参数，`a0`保存系统调用的返回值，寄存器`a7`用来传递syscall id。

