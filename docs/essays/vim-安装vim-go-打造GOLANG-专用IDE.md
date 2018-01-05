# vim 安装vim-go 打造GOLANG 专用IDE

---

## 分两步:
### 第一步：
    安装vim插件管理器Vundle
### 第二步：
    安装vim-go插件。

`另外：我也写了一个自动安装的脚本。手懒的朋友，可以自行下载使用：https://github.com/aimin/InstallvimGo.git`

## 开始：
### 第一步：安装Vundle

根据Vundle的安装说明，首先安装Vundle：

``` bash
$ git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim 
```

然后对.vimrc进行配置，将Vundle的相关配置置在最开始处，下面只显示关于Vundle的相关配置：
对.vimrc进行配置，将Vundle的相关配置置在最开始处，下面只显示关于Vundle的相关配置（详细参考Vundle的README.MD)：

``` bash
	1. " -------------  
	2. " Vundle  
	3. " https://github.com/gmarik/Vundle.vim  
	4. " -------------  
	5.   
	6. set nocompatible              " be iMproved, required  
	7. filetype off                  " required  
	8.   
	9. " set the runtime path to include Vundle and initialize  
	10. set rtp+=~/.vim/bundle/Vundle.vim  
	11. call vundle#begin()  
	12. " alternatively, pass a path where Vundle should install plugins  
	13. "call vundle#begin('~/some/path/here')  
	14.   
	15. " let Vundle manage Vundle, required  
	16. Plugin 'gmarik/Vundle.vim'  
	17.   
	18. " The following are examples of different formats supported.  
	19. " Keep Plugin commands between vundle#begin/end.  
	20. " plugin on GitHub repo  
	21. ""Plugin 'tpope/vim-fugitive'  
	22. " plugin from http://vim-scripts.org/vim/scripts.html  
	23. ""Plugin 'L9'  
	24. " Git plugin not hosted on GitHub  
	25. ""Plugin 'git://git.wincent.com/command-t.git'  
	26. " git repos on your local machine (i.e. when working on your own plugin)  
	27. ""Plugin 'file:///home/gmarik/path/to/plugin'  
	28. " The sparkup vim script is in a subdirectory of this repo called vim.  
	29. " Pass the path to set the runtimepath properly.  
	30. ""Plugin 'rstacruz/sparkup', {'rtp': 'vim/'}  
	31. " Avoid a name conflict with L9  
	32. ""Plugin 'user/L9', {'name': 'newL9'}  
	33.   
	34. " Install Vim-go  
	35. Plugin 'fatih/vim-go'  
	36.   
	37. " All of your Plugins must be added before the following line  
	38. call vundle#end()            " required  
	39. filetype plugin indent on    " required  
	40. " To ignore plugin indent changes, instead use:  
	41. "filetype plugin on  
	42. "  
	43. " Brief help  
	44. " :PluginList       - lists configured plugins  
	45. " :PluginInstall    - installs plugins; append `!` to update or just :PluginUpdate  
	46. " :PluginSearch foo - searches for foo; append `!` to refresh local cache  
	47. " :PluginClean      - confirms removal of unused plugins; append `!` to auto-approve removal  
	48. "  
	49. " see :h vundle for more details or wiki for FAQ  
	50. " Put your non-Plugin stuff after this line 
```

### 第二步：安装vim-go (详细查看vim-go的README.MD)

`注意路径`

``` bash
git clone https://github.com/fatih/vim-go.git ~/.vim/bundle/vim-go
```

至此安装完成。
打开.go 文件看看效果吧！ 