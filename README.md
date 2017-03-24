# My Awesome Book

镜像版本: `php:7.1.2-fpm-alpine`

| Nginx Version | PHP Version | Alpine Version | Container Scripts |
| :--- | :--- | :--- | :--- |
| 1.11.10 | 7.1.2 | 3.4 | 0.2.6 |

对于git可配置环境变量：-e flag:

* **GIT\_REPO **: git仓库地址，比如：https://github.com/project/   ssh 方式： [git@github.com](mailto:git@github.com):project.git

* **GIT\_BRANCH ：**Select a specific branch \(optional\)

* **GIT\_EMAIL **: Set your email for code pushing \(required for git to work\)

* **GIT\_NAME **: Set your name for code pushing \(required for git to work\)

* **GIT\_USE\_SSH **: Set this to 1 if you want to use git over SSH \(instead of HTTP\), useful if you want to use Bitbucket instead of GitHub
* **SSH\_KEY **: Private SSH deploy key for your repository base64 encoded \(requires write permissions for pushing\)
* **GIT\_PERSONAL\_TOKEN **: Personal access token for your git account \(required for HTTPS git access\)
* **GIT\_USERNAME **: Git username for use with personal tokens. \(required for HTTPS git access\)
* **WEBROOT**: Change the default webroot directory from
  `/var/www/html`
  to your own setting（默认代码存放路径）
* **ERRORS **: Set to 1 to display PHP Errors in the browser\(PHP错误机制\)
* **HIDE\_NGINX\_HEADERS **: Disable by setting to 0, default behaviour is to hide nginx + php version in headers
* **PHP\_MEM\_LIMIT **: Set higher PHP memory limit, default is 128 Mb（PHP 设置内存最大限制）
* **PHP\_POST\_MAX\_SIZE **: Set a larger post\_max\_size, default is 100 Mb （PHP 设置传值最大上传大小\)

* **PHP\_UPLOAD\_MAX\_FILESIZE**: Set a larger upload\_max\_filesize, default is 100 Mb（PHP设置最大下载大小）
* **DOMAIN**: Set domain name for Lets Encrypt scripts\(设置访问地址\)
* **REAL\_IP\_HEADER**: set to 1 to enable real ip support in the logs
* **REAL\_IP\_FROM**: set to your CIDR block for real ip in logs
* **RUN\_SCRIPTS**: Set to 1 to execute scripts
* **PGID**: Set to GroupId you want to use for nginx \(helps permissions when using local volume\)
* **PUID**: Set to UserID you want to use for nginx \(helps permissions when using local volume\)
* **REMOVE\_FILES**
  : Use REMOVE\_FILES=0 to prevent the script from clearing out /var/www/html \(useful for working with local files\)\(挂载卷\)



