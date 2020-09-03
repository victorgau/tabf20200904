# Python應用於金融數據分析

在這份文件中，我條列出了2020/09/04預計在台灣金融研訓院特約講座要講的內容。

## Python簡介

投影片：https://bit.ly/3jWfEtR

[Python 使用環境](https://ipython.org/ipython-doc/3/development/how_ipython_works.html
)

[Colab](https://colab.research.google.com/) 簡介

Python的使用哲學

什麼是模組？什麼是套件？

Python的副檔名 (.py, .ipynb)	
* Python的Hello World… 使用LineNotify！

什麼是變數？

使用[Visualize Python](http://www.pythontutor.com/visualize.html#mode=edit)可以讓初學者稍微了解一下變數在記憶體中的狀況。

用 type() 可以看變數裡面有什麼樣的資料！

怎麼寫程式？
* 程式 = 資料結構 + 演算法
* 基本資料型態 (int, float, bool, str)
* 基本容器型別 (list, tuple, dict, set)
* 基本語法 (if statement, loops, functions, exception handling)

list的操作：
* indexing
* slicing
* for迴圈

物件導向程式設計(OOP)：

* 物件加個點(.)可以提示有那些方法可以用

## 從網路上讀取資料 + 分析資料

看一下開放資料的格式大約有哪些：.csv, .json, .xlsx

* [政府資料開放平台](https://data.gov.tw/)

簡單介紹一下 Pandas 的使用

* 讀取HTML表格
* DataFrame 跟 Series

讀取元大台灣五十成分股

* [元大投信](https://www.yuantaetfs.com/#/Home/Index) > 產品資訊 > 元大台灣卓越50基金
* https://www.yuantaetfs.com/api/StkWeights?date=&fundid=1066

讀取股價歷史資料

* 使用loc找出特定區間的股價歷史資料
* 使用 dict + symbol 存放股價歷史資料
* 計算投資報酬率
* 計算多檔股票投資報酬率

讀取公司基本資料

* [政府資料開放平台](https://data.gov.tw/)
* [上市公司基本資料](https://data.gov.tw/datasets/search?qs=%E4%B8%8A%E5%B8%82%E5%85%AC%E5%8F%B8%E5%9F%BA%E6%9C%AC%E8%B3%87%E6%96%99)
* https://mopsfin.twse.com.tw/opendata/t187ap03_L.csv

讀取公司財務報表

* [日盛 - 台積電(2330)資產負債表](http://jsjustweb.jihsun.com.tw/z/zc/zcp/zcpb/zcpb_2330.djhtm)

讀取共同基金資料

* [基金類別績效](https://www.sitca.org.tw/ROC/Industry/IN2421.aspx)
* 計算基金績效
  * 對特定欄位排序，再使用 head() + 整數除法找出排序在前的基金代號
  * 使用 set + 交集找出投資標的

基本面選股

* 元大台灣50成分股 + 財務報表資料

## 資料視覺化 (Optional)

* [pyecharts](https://github.com/pyecharts/pyecharts)
* plotly + cufflinks

## 下單API的介紹

* [shiaoji](https://sinotrade.github.io/)
