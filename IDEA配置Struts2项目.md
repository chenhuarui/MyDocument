<h3> Struts2：IDEA配置项目总结 </h3>

- 创建项目 -> java Enterprise -> Web Application -> Struts2

- <font color =red>在创建项目时候 导入本地的 jar(Use library) -> 存放的struts2 jar包 (struts-2.5.17-min)</font>

- 默认不会添加 web/WEB-INF 下的 web.xml
  Project Structure -> Facets -> Web -> 添加 web.xml 并设置路径(重要)

- 设置 web.xml 的过滤器即拦截器，截获 struts2 的请求

` ` 标准化(可以去下载的 struts2 的jar中找)：

    <filter>
    <filter-name>struts2</filter-name> 
    <filter-class>
    org.apache.struts2.dispatcher.filter.StrutsPrepareAndExecuteFilter
    </filter-class>
    </filter>
	<filter-mapping>
	<filter-name>struts2</filter-name>
	<url-pattern>/*</url-pattern>
	</filter-mapping>

- 补充：将Poject Structrue Problems -> fix (一键解决问题)

<br>
<table><tr><td bgcolor=yellow>一些问题集合：
<br>

   * 引入 jar 包 将 struts-default 等红字问题
	- 引入对应的jar (xxx.core...)
<br>
<br>

  * 在 struts2 jar 的缺少和多余都会出现问题



</td></tr></table>


