# web项目         -- 此分支开箱即用，详见下面配置步骤

### 个人网站项目，实现的功能如下：
- 博客、代码库、文件下载、留言、联系站长、友情链接、新版特性
- 登录注册、邮箱验证码、MD5加密
- 上传文件、下载文件和图片
- 新建、编辑和删除博客、代码
- 博客和代码目录分类显示
- 查看、修改个人资料及邮箱、头像
- 增加、修改、浏览新版特性
- 站内搜索博客、文章
- 查看网站所有用户(站长功能)
- 网站实时在线用户显示、历史访问人数统计

PC端网址：https://www.hemingsheng.cn ，移动端网址：https://m.hemingsheng.cn

------------

## 主要文件结构如下

- `docs` -> 说明文档，包括打包好的war包和部署步骤
- `web-core` -> 后端Java源代码（使用时需打成jar包放在web的lib下，或者在Eclipse中的`Java Biuld Path`和`Deploymeny Assembly`中添加）
- `web-mobile` -> 响应式界面源码（在web和移动端是响应式布局）
- `web-pc` -> pc端界面源码（非响应式布局）

------------

## 快速配置方法：

- 1、下载项目源码或者打包好的war包

- 2、按照docs文件夹里面的数据库配置步骤，导入脚本，需提前安装PostgreSQL数据库和创建一个数据库(自定义名称，如web)
    - 按照`docs/数据库部署文件夹`里面的步骤依次运行脚本即可
    
- 3、将项目导入Eclipse/IDEA，修改web-pc和web-mobile 下的config/db_connect_info.properties文件里的数据库配置
    - 如果是下载的zip压缩包，则不用导入，直接解压，得到`config`文件夹和war包，并修改db_connect_info.properties数据库配置

- 4、放在tomcat等容器下运行。并将config文件夹放在web目录的同级目录（和web项目在同一个文件夹下）

- 5、访问 localhost:8080即可（默认配置已去掉项目名称）
