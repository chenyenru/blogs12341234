- [ ] Multivariate Regression
	- [ ] Research on Variables
	- [ ] Confounding Variables
	- [ ] research about monthly vs. annual data (pros and cons of summarizing monthly data into annual data or repeat the annual data 12 times as monthly data)
	- [ ] pick one of the 題目 you come up with, the one you like the most, and write a background/introduction paragraph. The paragraph should present the relevant background info, the problem statement, and our proposed research. And you should also cite sources whenever possible.

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