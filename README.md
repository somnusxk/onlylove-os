这是第一次上传项目，由于之前想做个特效收藏的网站，自己一直想注册的域名，现在又续费啦，不知道又得等到何年何月 ，所以现在把代码托管到github上，希望能有更多的朋友提提意见，这是一个独立的项目，由于之前通过使用分布式搭建，在服务器上上传代码调试，内存小，访问慢等等各种原因吧，所以最终选择放弃了分布式搭建，不过过几天我会把分布式搭建的项目也共享出来，最后整理了这个独立的项目，在服务器
访问速度相对好一点了
<h2>项目介绍</h2>
基于Spring+SpringMVC+Mybatis敏捷开发系统架构，采用JAVA语言，具有卓越的通用性、高效性、平台移植性和安全性。

项目模块：文章管理，用户管理，后台管理员，数据采集管理，网页管理，权限管理，系统管理，网站管理等几个模块

分层设计：（数据库层，数据访问层，业务逻辑层，展示层）层次清楚，低耦合。

安全编码：用户提交所有数据，在服务器端都进行安全编码，防止用户提交非法脚本及SQL注入获取敏感数据等，确保数据安全。

密码加密：登录用户密码进行MD5两次加密并加标识加密，此加密方法是不可逆的。保证密文泄露后的安全问题。

强制访问 ：系统对所有管理端链接都进行用户身份权限验证，防止用户直接填写url进行访问。

<h3>组织结构</h3>

![package](https://github.com/somnusxk/onlylove-os/blob/master/package.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/%E8%B5%84%E6%BA%90.png?raw=true)

# **技术选型** #

## 后端技术: ##

<table>

<tbody><tr>
<th>技术</th>
<th>名称</th>
<th>官网</th>
</tr>



<tr>
<td>SpringMVC</td>
<td>MVC框架</td>
<td><a href="http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/#mvc" target="_blank">http://docs.spring.io/spring/docs/current/spring-framework-reference/htmlsingle/#mvc</a></td>
</tr>
<tr>
<td>Security</td>
<td>安全框架</td>
<td><a href="http://spring.io/spring-security" target="_blank">http://spring.io/spring-security</a></td>
</tr>
<tr>
<td>phantomjs</td>
<td>数据爬取</td>
<td><a href="http://phantomjs.org/download.html" target="_blank">http://phantomjs.org/download.html</a></td>
</tr>
<tr>
<td>Nexus</td>
<td>私服仓库</td>
<td><a href="http://www.sonatype.org/nexus/go" target="_blank">http://www.sonatype.org/nexus/go</a></td>
</tr>
<tr>
<td>MyBatis</td>
<td>ORM框架</td>
<td><a href="http://www.mybatis.org/mybatis-3/zh/index.html" target="_blank">http://www.mybatis.org/mybatis-3/zh/index.html</a></td>
</tr>
<tr>
<td>MyBatis Generator</td>
<td>代码生成</td>
<td><a href="http://www.mybatis.org/generator/index.html" target="_blank">http://www.mybatis.org/generator/index.html</a></td>
</tr>
<tr>
<td>PageHelper</td>
<td>MyBatis物理分页插件</td>
<td><a href="http://git.oschina.net/free/Mybatis_PageHelper" target="_blank">http://git.oschina.net/free/Mybatis_PageHelper</a></td>
</tr>
<tr>
<td>Druid</td>
<td>数据库连接池</td>
<td><a href="https://github.com/alibaba/druid" target="_blank">https://github.com/alibaba/druid</a></td>
</tr>
<tr>
<td>Redis</td>
<td>缓存数据库</td>
<td><a href="https://redis.io/" target="_blank">https://redis.io/</a></td>
</tr>
<tr>
<td>Solr &amp; Elasticsearch</td>
<td>分布式全文搜索引擎</td>
<td><a href="http://lucene.apache.org/solr/" target="_blank">http://lucene.apache.org/solr/</a> <a href="https://www.elastic.co/" target="_blank">https://www.elastic.co/</a></td>
</tr>
<tr>
<td>Quartz</td>
<td>作业调度框架</td>
<td><a href="http://www.quartz-scheduler.org/" target="_blank">http://www.quartz-scheduler.org/</a></td>
</tr>
<tr>
<td>RabbitMQ</td>
<td>消息队列</td>
<td><a href="http://www.rabbitmq.com/" target="_blank">http://www.rabbitmq.com/</a></td>
</tr>

<tr>
<td>Log4J</td>
<td>日志组件</td>
<td><a href="http://logging.apache.org/log4j/1.2/" target="_blank">http://logging.apache.org/log4j/1.2/</a></td>
</tr>
<tr>
<td>Swagger2</td>
<td>接口测试框架</td>
<td><a href="http://swagger.io/" target="_blank">http://swagger.io/</a></td>
</tr>

<tr>
<td>Maven</td>
<td>项目构建管理</td>
<td><a href="http://maven.apache.org/" target="_blank">http://maven.apache.org/</a></td>
</tr>

</tbody></table>

## 前端技术: ##
<table>

<tbody><tr>
<th>技术</th>
<th>名称</th>
<th>官网</th>
</tr>


<tr>
<td>jQuery</td>
<td>函式库</td>
<td><a href="http://jquery.com/" target="_blank">http://jquery.com/</a></td>
</tr>
<tr>
<td>Bootstrap</td>
<td>前端框架</td>
<td><a href="http://getbootstrap.com/" target="_blank">http://getbootstrap.com/</a></td>
</tr>
<tr>
<td>Bootstrap-table</td>
<td>Bootstrap数据表格</td>
<td><a href="http://bootstrap-table.wenzhixin.net.cn/" target="_blank">http://bootstrap-table.wenzhixin.net.cn/</a></td>
</tr>
<tr>
<td>Font-awesome</td>
<td>字体图标</td>
<td><a href="http://fontawesome.io/" target="_blank">http://fontawesome.io/</a></td>
</tr>
<tr>
<td>multi-select</td>
<td>选择框</td>
<td><a href="http://loudev.com/" target="_blank">http://loudev.com/</a></td>
</tr>
<tr>
<td>jquery.fileupload</td>
<td>文件上传</td>
<td><a href="https://github.com/blueimp/jQuery-File-Upload/" target="_blank">https://github.com/blueimp/jQuery-File-Upload/</a></td>
</tr>
</tbody></table>

# **环境搭建** #
## 开发工具: ##

MySql: 数据库

Tomcat: 应用服务器

SVN|Git: 版本管理

Nginx: 反向代理服务器

spring tool suite: 开发IDE

PowerDesigner: 建模工具

Navicat for MySQL: 数据库客户端

## 开发环境： ##
jdk8

Mysql 6.0.6

Redis

Rabbitmq

nexus

Linux

## 工具安装 ##
由于是在linux安装，安装步骤我这边就省略了，如果有需要可以加我qq：915719960

## 开发指南: ##
1，在自己机器上按照以上用到的工具进行安装并启动相关服务即可。

2，下载源代码到本地并打开本地编译并安装到本地maven仓库

## 部署方式 ##
1，war包项目：使用tomcat等web容器启动

## 演示地址 ##

演示地址：http://192.168.99.116:8099/admin/index

如果想通过线上地址访问查看，由于服务器上一些其他信息，所以暂时不公开地址，如果有需要的可以加QQ

## 预览图 ##
![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E6%88%AA%E5%9B%BE20170619153143.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E5%9B%BE%E7%89%8720170619161622.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E6%88%AA%E5%9B%BE20170619153232.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E6%88%AA%E5%9B%BE20170619153349.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E6%88%AA%E5%9B%BE20170619153604.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E5%9B%BE%E7%89%8720170619153859.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E5%9B%BE%E7%89%8720170619172634.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E5%9B%BE%E7%89%8720170619172932.png?raw=true)

![package](https://github.com/somnusxk/onlylove-os/blob/master/QQ%E5%9B%BE%E7%89%8720170619153647.png?raw=true)

<font color="red">最后一张图片是通过爬取其他网站特效，希望不要影响到大家的浏览</font>

至此，关于数据库建模的图片我这边就不上传了，到时可以根据sql脚本进行执行

另外：数据爬取到时更新代码会把他摘取掉，由于时间原因今天就先写到这，明天整理更新代码提交

# **关于数据爬取** #
由于数据爬取刚接触，只是写了几个简单脚本抓取《推酷》《51CTO博客》《CSDN博客》《天涯社区》《博客园》通过代码转换成系统所需要的数据，对图片进行判断获取替换成本系统能查看的图片。只是为了增加调试查看方便。所以数据爬取代码不会更新，如有想交流的朋友可以加我QQ

# **在线文档** #
<ul class="task-list">
<li><p><a href="http://tool.oschina.net/apidocs" title="在线Api帮助文档" target="_blank">在线Api帮助文档</a></p></li>
<li><p><a href="http://tool.oschina.net/apidocs/apidoc?api=jdk_7u4" title="JDK7英文文档" target="_blank">JDK7英文文档</a></p></li>
<li><p><a href="http://spring.oschina.mopaas.com/" title="Spring4.x文档" target="_blank">Spring4.x文档</a></p></li>
<li><p><a href="http://www.mybatis.org/mybatis-3/zh/index.html" title="Mybatis3官网" target="_blank">Mybatis3官网</a></p></li>

<li><p><a href="http://tool.oschina.net/apidocs/apidoc?api=nginx-zh" title="Nginx中文文档" target="_blank">Nginx中文文档</a></p></li>
<li><p><a href="http://freemarker.foofun.cn/" title="Freemarker在线中文手册" target="_blank">Freemarker在线手册</a></p></li>

<li><p><a href="http://www.bootcss.com/" title="Bootstrap在线手册" target="_blank">Bootstrap在线手册</a></p></li>
<li><p><a href="https://git-scm.com/book/zh/v2" title="Git官网中文文档" target="_blank">Git官网中文文档</a></p></li>

</ul>

