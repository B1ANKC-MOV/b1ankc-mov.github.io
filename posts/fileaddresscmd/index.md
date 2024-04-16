# [汇总] cd打开文件命令&文件相对路径写法

在控制台中输入指令打开文件路径和在项目中输入文件路径的一些写法经常容易混淆记错，因此在这里汇总一下，方便以后查询记忆。

## 控制台终端打开文件
1. 在搜索框中搜索“cmd”或按<kbd>win</kbd>+<kbd>R</kbd>打开命令窗口，在默认路径后输入“cd”+空格，再输入指定文件夹路径。

   如果回车后暂时还是原来默认的路径，则输入指定文件夹所在的盘再回车即可，例如：`D:`。

2. 打开指定的文件夹，在路径栏里输入“cmd”，回车进入控制台。默认路径就是指定文件夹的路径

3. 打开指定的文件夹，按住<kbd>shift</kbd>在空白处右击，在菜单栏中选择***在此处打开Powershell窗口***（可能有人的选项是*在此处打开命令窗口*）
   <!--more-->

## cd命令符号表

| 命令       | 操作结果                     |
| ---------- | ---------------------------- |
| `cd /`     | 进入根目录                   |
| `cd .`     | 单纯表示当前目录             |
| `cd ./`    | 打开当前目录下文件/文件夹    |
| `cd ..`    | 返回上一级目录               |
| `cd ../..` | 返回上两级目录               |
| `cd ~`     | 进入当前用户默认目录         |
| `cd -`     | 返回进入此目录之前的目录位置 |

{{< admonition tip >}}

对于`cd ./`，如当前目录下一文件夹名为mnt，`cd ./mnt`或`cd mnt`都可进入该文件夹

{{< /admonition>}}

## 文件相对路径写法

### 当前目录或下级目录

- 引用当前文件所在目录下名为data.txt的文件：`data.txt`或`./data.txt`

- 引用当前文件所在目录的images文件夹中的logo.png文件：`images/logo.png`或`./images/logo.png`

### 上级目录或上上级目录

- 引用当前文件所在目录的上级目录中名为data.txt的文件：`../data.txt`

- 引用当前文件所在目录的上上级目录中名为data.txt的文件：`../../data.txt`

### 根目录

- 引用项目根目录下名为data.txt的文件：`/data.txt`

- 引用项目根目录下的images文件夹中的logo.png文件：`/images/logo.png`



