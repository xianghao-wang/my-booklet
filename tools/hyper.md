---
description: Hyper YYDS
---

# 好看的Terminal

## 展示

![](../assets/01-hyper-01.png)

## 环境

* Macbook Pro M1 Max 2021
* Macbook Pro 16-inch 2019
* shell解释器 为**zsh**

## 准备

* 安装**Hyper** [here](https://hyper.is)
* 安装**oh-my-zsh** [here](https://ohmyz.sh/#install)

## 配置oh-my-zsh

### 语法高亮和自动补全

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

### 主题

```bash
vi ~/.zshrc

# 修改ZSH_THEME后的面的主题为ys
ZSH_THEME="ys"

# 修改后关闭.zshrc并重新加载
source ~/.zshrc
```

## 美化Hyper

```bash
# 打开hyper配置文件
vi ~/.hyper.js

# 向plugins添加hyper-snazzy
plugins: [
    "hyper-snazzy"
]

# 保存后，重启Hyper即可修改成功
```

