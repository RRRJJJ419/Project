建了一個簡單的個人理財網頁伺服器練習環境，實踐 Python Flask 、從 API 調取匯率及台股股價的即時資料，且將輸入的資料存入資料庫，在前端顯示個人財務紀錄及股票庫存損益，並將儲存資料做視覺化圖表的呈現。

# **db_setting.py**

![image](https://github.com/user-attachments/assets/f2ee5a69-3983-489c-b2e4-9b935259081a)

用sqlite3創建現金/股票資料庫儲存輸入的資料

![image](https://github.com/user-attachments/assets/36494d2d-6fef-42bd-a67d-36001a612d5c)

# **index.py**

![image](https://github.com/user-attachments/assets/9c317b9c-1b40-4b5a-a873-7c842937360f)

主程式:
網頁伺服器(Flask)建立、與資料庫連接儲存提交的資訊到資料庫、使用匯率API獲取台幣美金匯率及證交所API獲取股票資訊(含後續計算市值、成本、報酬率等內容)、繪製資產及股票分布圓餅圖、對伺服器提交資料並更新資料庫(含刪除)



# **templates資料夾**
![image](https://github.com/user-attachments/assets/c1ea5fdf-cb19-4d28-8518-411e7f1360ef)

## **index.html**
![image](https://github.com/user-attachments/assets/86094275-7dd6-4eb4-9c53-96b22daf8a79)

網頁主頁面:
顯示現金庫存、現金更動紀錄(含刪除按鈕功能)、股票庫存(含刪除功能)、股票庫存占比圖、資產比例占比圖

## **base.html**
![image](https://github.com/user-attachments/assets/47984270-3cec-4f19-9a9c-ae5192f933a1)

網頁頁面中固定不動/每個子分頁會重複的地方(navbar):

![image](https://github.com/user-attachments/assets/f3edac60-dcfe-4eb3-ae12-0b8d3a6c7f34)

## **cash.html**
![image](https://github.com/user-attachments/assets/5c121474-b29c-428b-92ee-1dd580a53ca6)

現金庫存頁面(提交新增現金資訊表單)

## **stock.html**
![image](https://github.com/user-attachments/assets/df0d6988-a7f9-4d2d-b974-01e28c0df14c)

股票庫存頁面(提交新增股票買入資訊表單)




