<a href="http://www.sublimetext.com/3" target="_blank">官方下载地址</a>
* version: Sublime Text Build 3047 x64

SublimeText3-Usage
==================

   Sublime Text 3 是一款具有代码高亮、语法提示、自动完成且反应快速的编辑器软件，不仅具有华丽的界面，还支持插件扩展机制，用她来写代码，绝对是一种享受。
　

   作者很大方, 不注册照样使用, 唯一的遗憾是当保存文件到达一定次数的时候会弹出一个框框提示你木有注册并请注册.

##视频简介(中文)
* http://v.youku.com/v_show/id_XMzU5NzQ5ODgw.html

##插件仓库
* https://sublime.wbond.net/installation#st3 

##安装插件控制器package controller
1. menu -> view -> show console
1. 从插件仓库中获得st3安装代码(import ....) 在console中执行即可


##使用插件控制器
* ctrl + shift + p -> package control: Install(curd) package

##LZ已安装并测试OK的插件
1. ConvertToUTF8         :二选一解决GBK支持
1. less 	         : less语法高亮
1. Less2css		 : less编译为css
1. Better CoffeeScript   : Syntax highlighting and checking, commands, shortcuts, snippets, watched compilation and more.
1. jQuery 		 : 不解释
1. html5		 : 更多标签提示
1. tag			 : 类似html5增强提供更多的标签.
1. bootstrap3		 : 有他不用再去官网copy代码
1. angularjs		 : 代码块提示
1. Emmet		 : 原名ZenCoding, div#container>ul>li*4 生成class为container的div,下一ul并且其下有四个li
1. HTML-CSS-JS Prettify  : 代码格式化, 打开文件右键设置指定 nodejs.exe 文件路径
1. SideBarEnhancements	 : 边侧栏增强
1. DocBlockr 		 : 生成js注释, 很强大
1. bracketHighlighter	 : 区域内括号高亮显示
1. svn or TortoiseSVN	 : 前者文本信息显示与提示, 后者需要设置 TortoiseProc.exe, 推荐后者
1. Markdown preview      : 生成临时 html 预览 ,命令:mark** in browser
1. autoprefixr		 : 前缀 css 浏览器兼容, 命令 autoprefixr 自动补代码
1. Tradsim		 : 中文繁字体和简体字转换 ,命令:Tradsim xxx
1. TrailingSpaces	 : 多于空格高亮显示(洁癖)
1. Alignment		 : 变量等号"="对齐(洁癖)


##待安装试验的插件:
1. JsMinifier: 该插件基于Google Closure compiler，自动压缩js文件。(https://github.com/cgutierrez/1sMinifier/issues)
1. SublimeCodeIntel: 代码自动提示
1. Clipboard History: 粘贴板历史记录，方便使用复制/剪切的内容。 (st2 OK , 3 nosearch)
1. htmlBeautiful: ctrl + shift +alt + f (js_format too) (st2 OK , 3 nosearch) html格式化
1. JsFormat(removed)
1. fileDiffs: 区分文件内容不同 (用处不大)
1. jsHint: 校验js错误 (太严谨, 不实用)
1. sublime TODD: 当前文件..(no search)
1. sublime v8: 控制台, js 调试之类.. (no search)

##基础设置

```json
	{
	    "line_numbers": true,               //是否显示行号
	    "gutter": true,                     //是否显示边列
	    "draw_centered": false,             //是否居中显示
	    "wrap_width": 170,                  //换行宽度(单位：字符)
	    "word_wrap": true,                  //是否自动换行
	    "scroll_past_end": true,            //滚动能否超过结尾
	    "font_face": "Consolas YaHei",      //字体
	    "font_size": 11,                    //字体大小
	    "line_padding_top": 1,              //行高
	    "line_padding_bottom": 1,
	    "tab_size": 2,                      //TAB缩进宽度
	    "translate_tabs_to_spaces": false,  //自动转换TAB为空格
	    "update_check": false,              //禁用自动更新
	    "theme": "Soda Dark 3.sublime-theme"//皮肤
	}
```


##内置快捷键
* Ctrl+Shift+P：打开命令面板
* Ctrl+P：搜索项目中的文件
* Ctrl+G：跳转到第几行
* Ctrl+W：关闭当前打开文件
* Ctrl+Shift+W：关闭所有打开文件
* Ctrl+Shift+V：粘贴并格式化
* Ctrl+D：选择单词，重复可增加选择下一个相同的单词
* Ctrl+L：选择行，重复可依次增加选择下一行
* Ctrl+Shift+L：选择多行
* Ctrl+Shift+Enter：在当前行前插入新行
* Ctrl+X：删除当前行
* Ctrl+M：跳转到对应括号
* Ctrl+U：软撤销，撤销光标位置
* Ctrl+J：选择标签内容
* Ctrl+F：查找内容
* Ctrl+Shift+F：查找并替换
* Ctrl+H：替换
* Ctrl+R：前往 method
* Ctrl+N：新建窗口
* Ctrl+K+B：开关侧栏
* Ctrl+Shift+M：选中当前括号内容，重复可选着括号本身
* Ctrl+F2：设置/删除标记
* Ctrl+/：注释当前行
* Ctrl+Shift+/：当前位置插入注释
* Ctrl+Alt+/：块注释，并Focus到首行，写注释说明用的
* Ctrl+Shift+A：选择当前标签前后，修改标签用的
* F11：全屏
* Shift+F11：全屏免打扰模式，只编辑当前文件
* Alt+F3：选择所有相同的词
* Alt+.：闭合标签
* Alt+Shift+数字：分屏显示
* Alt+数字：切换打开第N个文件
* Shift+右键拖动：光标多不，用来更改或插入列内容
* 按Ctrl，依次点击或选取，可需要编辑的多个位置 (列模式)
* 按Ctrl+Shift+上下键，移动行

##列选择模式
1. 按住Ctrl点击鼠标左键，就会出现多个光标指针，或能选择多处文本，然后就可以批量编辑或输入。
1. 按住shift，右键可以拖拽选区。
1. 光标放在某处，按住Ctrl+Alt+Up键，或Ctrl+Alt+Down键，光标能上下延伸，然后左右键可移动.

##Ubuntu下搜狗输入法中文输入问题
1. 先安装， 官方下载deb，或者 sudo apt-get install sublimt-text
2. 卸载： sudo apt-get remove sublimt-text，sudo dkpg -r sublime-text
3. 安装编译环境
4. sudo apt-get install build-essential
5. sudo apt-get install libgtk2.0-dev
6. 下载sublime-imfix.c源文件： http://pan.baidu.com/s/1eQcPeE2 ， 如果链接失效请给邮件联系我。
7. 进入该文件所在目录编译该文件，命令：gcc -shared -o libsublime-imfix.so sublime-imfix.c  `pkg-config --libs --cflags gtk+-2.0` -fPIC
8. 在其目录下将编译生产的libsublime-imfix.so拷贝到sublime的安装目录下,命令：sudo cp ./libsublime-imfix.so /opt/sublime-text
9. sudo vim /usr/bin/subl, 在exec上面一行加入： export LD_PRELOAD=/opt/sublime_text/libsublime-imfix.so
10. 修改: sudo vim /usr/share/applications/sublime_text.desktop , Exec=/opt/sublime-text/sublime-text改为： Exec=/usr/bin/subl
11. 完成， 重新打开sublime测试即可。
