tmuxen
------

轻易创建 tmux 使用环境。

![tmux](https://github.com/xuxiaodong/tmuxen/raw/master/screenshot.png)

## 安装

    git clone git://github.com/xuxiaodong/tmuxen.git
    ./install-tmuxen

## 使用

    tmuxen
## 重启保存恢复
参照[重启和恢复tmux回话](https://liam.page/2016/09/10/tmux-plugin-resurrect/) 

主要是要安装一个`tumx-resurrect` 的插件, 安装插件需要用到插件管理器`Tmux Plugin Mange` , Github地址为`https://github.com/tmux-plugins/tpm` 将`Tmux Plugin Mange` 克隆到本地。
```
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

`.tumx.config` 中已经包含了需要添加的插件名称。克隆完成后，需要安装插件,在你的终端执行完`./install-tmuxen` 后需要重新`tumx soucrce ~/.tmux.conf` 重新加载下配置文件，`tumux` 安装插件的方式是使用`Prefix` + `I` , 我们现在设置的`Prefix` 是`C-s` 

记住一下命令：
| 命令            | 功能          |
| --------------- | ------------- |
| `Prefix+I`      | 安装插件      |
| `Prefix+U`      | 更新插件      |
| `Prefix+alt+u`  | 卸载插件      |
| `Prefix+<C-s>`  | 保存回话状态  |
| `prefix+<C-r>`  | 恢复回话状态  |

记住经常使用`Prefix+<C-s>` 来保存回话
### tmux 复制到系统剪切板
进入复制模式，选择需要复制的内容，直接`Enter` 就可以将选择内容复制到系统剪切板
