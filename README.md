# 百度地图数据采集工具使用说明

## 功能和项目文档结构：
1.功能
>(1).根据关键词（街道、酒店或其他标志性建筑物等），查询周边的商户、酒店、交通位置等兴趣点  
(2).使用PyQt5可视化选择抓取选项与抓取结果并可以对抓取结果进行动态编辑  
>(3).抓取结果导出为Excel表格  

2.项目结构
>
├── ChinaArea 全国省市数据  
│   ├── China_area.py  
│   └── __init__.py  
├── Crawler 爬虫程序  
│   ├── BaiduMapCrawler.py    
│   └── __init__.py  
├── main.py 主程序  
├── Mainwindow Ui界面文件  
│   ├── __init__.py  
│   └── Mainwindow.py  
├── qtpandas_1.0.4_v2 修正后的qtpandas安装包   
├── README.md 项目文档说明  
├── requirements.txt 依赖包    
└── resource 资源文件  
    ├── image 界面加载图标以及程序运行截图  
    │   ├── run_main.gif  
    │   ├── spider2.png  
    │   ├── spider3.png  
    │   ├── spider.png  
    │   ├── 导出结果界面.jpg  
    │   ├── 启动界面.jpg    
    │   ├── 抓取结果.jpg  
    │   └── 抓取时界面.jpg  
    └── QSS  
        └── Mainwindow.qss  
>

## 依赖库
1.requirements.txt（可以直接使用pip install requirements.txt安装）
>certifi==2017.7.27.1  
chardet==3.0.4  
et-xmlfile==1.0.1  
future==0.16.0  
idna==2.6  
jdcal==1.3  
numpy==1.13.3  
openpyxl==2.4.9  
pandas==0.20.3  
PyQt5==5.9  
python-dateutil==2.6.1  
pytz==2017.2  
QtPy==1.3.1  
requests==2.18.4  
sip==4.19.3  
six==1.11.0  
>urllib3==1.22  

2. 修正过的qtpandas  
>qtpandas在github上的最新版本代码有问题，需要修正  
请下载本项目下修正过的qtpandas代码安装
> 之前写这个小程序时给qtpandas提交了这个问题的issue,

2018年8月，收到邮件，已经修复这个bug.
可以直接在github上搜索qtpandas，然后 ```pip install .```安装，或者```python setup.py```
安装，也可以cd到本程序所在目录里的qtpandas_1.0.4中使用pip安装。
>对应目录：qtpandas_1.0.4

## 使用说明
1.执行 python run.py，程序启动界面如下  
![Alt text](./resource/image/启动界面.jpg)  

2.选择省、市，然后输入关键词，例：四川省 成都市 天府广场 
![Alt text](./resource/image/run_main.gif)  
 

3.导出抓取结果为excel表格  
![Alt text](./resource/image/导出结果界面.jpg)



