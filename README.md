## 日期函式
moment().format('YYYY-MM-DD HH:mm:ss')

## 氣象 API
網址： https://opendata.cwb.gov.tw/api/v1/rest/datastore/F-D0047-093
### 參數
#### Authorization 
CWB-8065CE03-95E7-4162-A6F3-D5E022F1A81C
#### format
JSON
#### locationId
F-D0047-033
#### locationName
內埔鄉
#### elementName
AT,CI,PoP6h,MinCI,MaxAT,MaxCI,MinT,UVI,MinAT,MaxT,WS,WD,Td,PoP12h,T,RH,Wx,WeatherDescription

## 整理氣象資料程式碼
tmp.weatherInfo = JSON.stringify(tmp.data)
tmp.rainRate = tmp.data.records.locations[0].location[0].weatherElement[0].time[0].elementValue[0].value

## 簡報
https://drive.google.com/file/d/1URwyYxjLwiw9hHbCQgwV8hyfGIV-MyqR/view?usp=sharing

