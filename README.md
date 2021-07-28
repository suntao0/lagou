# lagou
通过python爬虫利用requests模块爬获拉勾网数据下载并保存
 前言
本文从拉勾网爬取深圳市数据分析的职位信息，并以xls格式保存至电脑。

1. 用到的软件包
Python版本： Python3.6/3.7
requests: 下载网页
josn:分析并转换数据
time: 暂停进程
xlwt:数据以xls格式文件保存
2. 解析网页
打开Chrome,在拉勾网搜索某市的公司,使用检查功能查看网页源代码,发现拉勾网有反爬虫机制, 职位信息并不在源代码里,而是保存在JSON的文件里,因此我们直接下载JSON,并使用字典方法直接读取
数据.
抓取网页时,需要加上头部信息, 才能获取所需的数据.
3. 保存数据
通过爬取数据以后可以利用xls模块下载并保存下来了
