Candy
=====

Candy : A New Tool for quick open files and fast search text.

2.0.0.6:
	修改：GeneralSettings.ini 里面两个段的写法，感谢群友指出原写法不易读。具体如下：
		[LineJumpArgs_for_TextEditor]====>[TextEditor's_CommandLine]
		[ProfileArgs_For_WebBrowser]====>[WebBrowser's_CommandLIne]
	修改：单词的写法错误，请把GeneralSettings.ini里面的Deault_TextEditor改成Default_TextEditor
	修正：一个函数的用法错误。导致没有定义默认文本编辑器时，报错。
	删减：去掉关于管理员的权限的判断，避免非管理员运行出错。
	增加：一个简单的托盘菜单
	修正：Config命令重新修正为“编辑所有相关ini”
	
2.0.0.5:
	增强：进入配置时能够跳转到相应的行的配置写法，以便适应大部分流行文本编辑器。命令行写法参见本次附带的ini
	修改：将环境变量.ini与热键设置.ini 合并成GeneralSettings.ini。同时这个文件里面的所有中文变量，修改成英文写法，请对照修改。
	修改：原来部分Gloabal的参数为非全局，以便即时修改。
	
2.0.0.4:
	增加：进入配置时，能够跳转到相应的行。
	
2.0.0.3:
	修正：对文件夹，取ParentName，遇到含 . 文件夹名字会出错的问题。
	修改：由于Candy的INI可以来自多个ini文件，为了快速定位某条设定所在的ini。Candy重新设计为：按住Ctrl键，点任意菜单条，打开该条菜单所在ini文件。
	     按住Ctrl键，点第一条菜单项，进入“主配置ini”所在文件。
	
	
2.0.0.2:
	修改：Clip“命令”与“开关”的写法都改回SetClipBoard
	修正：多文件时，取ParentName，遇到含 . 文件夹名字会出错的问题。
	修正：环境变量里面如果有不规范变量名，程序出错。改成如果有不规范名，则抛弃该条定义。
	增加：CandySelected与CandySel同样可以用于Cando脚本，兼容以前的cando变量写法
