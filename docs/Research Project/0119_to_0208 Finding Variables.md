- [ ] Multivariate Regression
	- [ ] Research on Variables
	- [ ] Confounding Variables
	- [ ] research about monthly vs. yearly data (pros and cons of summarizing monthly data into annual data or repeat the annual data 12 times as monthly data)
	- [ ] pick one of the 題目 you come up with, the one you like the most, and write a background/introduction paragraph. The paragraph should present the relevant background info, the problem statement, and our proposed research. And you should also cite sources whenever possible.
# AQI
First up, what is AQI?
![基於備選傳感器和預測模型的空氣質量試驗](https://aqicn.org/air/experiments/images/aqiscale.png)

### Calculations ([source](https://tw.piliapp.com/aqi/tw/))
先由下列方法來計算出各種副指標值：

-   O3,8hr： 取最近連續8小時移動平均值
-   O3： 取即時濃度值
-   PM2.5： 0.5 × 前12小時平均 + 0.5 × 前4小時平均
-   PM10： 0.5 × 前12小時平均 + 0.5 × 前4小時平均
-   一氧化碳： 取最近連續8小時移動平均值
-   二氧化硫： 取即時濃度值
-   二氧化硫24小時： 取最近連續24小時濃度平均值
-   二氧化氮： 取即時濃度值

再依 **污染物濃度與即時副指標值對照表** 來找出最大的做為 AQI
![[截圖 2022-02-06 下午12.36.51.png]]
台灣的即時空氣品質指標(AQI)計算方式為： O3 (臭氧)、PM2.5 (細懸浮微粒)、PM10 (懸浮微粒)、CO (一氧化碳)、SO2 (二氧化硫)、 NO2 (二氧化氮) 依不同的時間長度來計算出一個指標值，再取出其中最大值為即時空氣品質指標，該最大值測項即為指標污染物。


# Variables
- 台中市
	- 主要死因
		- 氣管、支氣管、肺癌
>colnames(merged)
 [1] "year"                                                   
 [2] "死亡人數-主要死因_癌症(人)_男"                          
 [3] "死亡人數-主要死因_癌症(人)_女"                          
 [4] "死亡人數-主要死因_肺炎(人)_男"                          
 [5] "死亡人數-主要死因_肺炎(人)_女"                          
 **[6] "死亡率-主要癌症_氣管、支氣管和肺癌_死亡率(人/十萬人)_男"
 [7] "死亡率-主要癌症_氣管、支氣管和肺癌_死亡率(人/十萬人)_女"**
 [8] "標準化死亡率-主要死因_總計(人/十萬人)_男"               
 [9] "標準化死亡率-主要死因_總計(人/十萬人)_女"               
[10] "標準化死亡率-主要死因_癌症(人/十萬人)_男"               
[11] "標準化死亡率-主要死因_癌症(人/十萬人)_女"               
[12] "空氣中總懸浮微粒濃度"                                   
[13] "細懸浮微粒手動監測(PM2.5)濃度值"                        
[14] "空氣中臭氧濃度"                                         
[15] "二氧化硫含量"                                           
[16] "AQI(PSI)>100之日數比率"      

6, 7 are the dependent variables i wish to investigate on
and other variables are used as **confounding variables**
- 
# Monthly vs Yearly Data
![[withers2015.pdf]]

According to Withers, 
>To answer the question in the title, we suggest the following rough rule: use annual means if 5 or more years of data are available; and use monthly means if less than 5 years of data are available

Thus, _I'll use annual means because my data contains more than 5 years of records_
# Topic
I'm interested in whether air quality index 