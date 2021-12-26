---
description: Hyper YYDS
---

# 好看的Terminal

## <span id='presentation'>展示</span>

![](../assets/01-hyper-01.png)

## <span id='environment'>环境</span>

* Macbook Pro M1 Max 2021
* Macbook Pro 16-inch 2019
* shell解释器 为**zsh**

## <span id='preperation'>准备</span>

* 安装**Hyper** [here](https://hyper.is)
* 安装**oh-my-zsh** [here](https://ohmyz.sh/#install)

## <span id='oh-my-zsh'>配置oh-my-zsh</span>

### <span id='oh-my-zsh-01'>语法高亮和自动补全</span>

下载**zsh-syntax-highlighting**和**zsh-completions**插件

```bash
# 将语法高亮插件下载到插件文件见
cd ~/.oh-my-zsh/custom/plugins
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
git clone https://github.com/zsh-users/zsh-completions.git
```

打开`.zshrc`, 配置插件

```bash
vi ~/.zshrc
```

看到如下`plugins`, 像里面添加`zsh-syntax-highlighting`和`zsh-completions`

```bash
plugins={
    git
    zsh-syntax-highlighting
    zsh-completions    
}
```

重新加载`.zshrc`

```
source ~/.zshrc
```

### <span id='oh-my-zsh-02'>主题</span>

```bash
vi ~/.zshrc

# 修改ZSH_THEME后的面的主题为ys
ZSH_THEME="ys"

# 修改后关闭.zshrc并重新加载
source ~/.zshrc
```

## <span id='hyper'>美化Hyper</span>

```bash
# 打开hyper配置文件
vi ~/.hyper.js

# 向plugins添加hyper-snazzy
plugins: [
    "hyper-snazzy"
]

# 保存后，重启Hyper即可修改成功
```

## <span id='sf'>screenfetch - 在终端中显示系统图标及参数</span>

* 安装**screenfetch**

```sh
# 使用homebrew安装
brew install screenfetch
```

* 打开终端时自动启动screenfetch

```sh
# 打开.zshrc
vi ~/.zshrc

# 在里面加入
screenfetch
```

