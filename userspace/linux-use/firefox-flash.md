# firefox 安装flash插件


火狐浏览器默认情况下是不带 flash_player，一般情况下有flash的网页打开就会提示安装flash_player插件。

* 先根据火狐的提示，去ADOBE的网站下载 install_flash_player_10_linux.tar.gz
* tar -zxvf install_flash_player_10_linux.tar.gz  
* 解压后得到一个动态库文件 libflashplayer.so，将其复制到火狐插件目录下:

&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;cp libflashplayer.so /usr/lib/mozilla/plugins

&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;此目录可能根据火狐不同的版本有所不同，大家可以先去lib下面搜索一下mozilla;

* 将libflashplayer.so复制进去之后，重启firefox,接下来看看网页就知道生效了;