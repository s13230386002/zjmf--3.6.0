1.首先需要安装php扩展。根据网站要使用的php版本，下载扩展文件（php7.2、php7.3、php7.4），上传到php安装目录 /lib/php/extensions/no-debug-non-zts-xxxx（xxxx为一串数字）文件夹里面。

2.修改php配置文件（php.ini），加入以下内容，然后重启php进程。

extension=idcsmart.so
3.使用官方安装包进行安装。填写授权码的时候，随便填写一个的32位大写的MD5字符串，例如可以在这里生成。（之前安装过的可以跳过此步骤）

安装完之后默认就是专业版，所有专业版的功能均可使用。

如果上传了第三方付费插件或模板，使用过程中提示插件未购买，需要在php配置文件（php.ini）加入idcsmart.app这个配置项，配置第三方插件标识，多个插件标识用英文逗号隔开，例如：

idcsmart.app=AliPayDmf,Smsbao,Subemail
重启php进程，在后台系统升级页面，已授权模块处，点击“拉取授权”。即可使用付费的第三方插件或模板。