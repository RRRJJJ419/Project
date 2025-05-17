建了一個簡單的個人理財網頁伺服器練習環境，實踐 Python Flask 、從 API 調取匯率及台股股價的即時資料，且將輸入的資料存入資料庫，在前端顯示個人財務紀錄及股票庫存損益，並將儲存資料做視覺化圖表的呈現。

# **db_setting.py**

![image](https://github.com/user-attachments/assets/f2ee5a69-3983-489c-b2e4-9b935259081a)

用sqlite3創建現金/股票資料庫儲存輸入的資料

![image](https://github.com/user-attachments/assets/36494d2d-6fef-42bd-a67d-36001a612d5c)

# **index.py**

![image](https://github.com/user-attachments/assets/9c317b9c-1b40-4b5a-a873-7c842937360f)

主程式:
網頁伺服器(Flask)建立、與資料庫連接儲存提交的資訊到資料庫、使用API獲取台幣美金匯率及股票資訊(含計算市值、成本、報酬率等內容)、繪製資產及股票分布圓餅圖、對伺服器提交資料並更新資料庫(含刪除)



# **templates資料夾**
![image](https://github.com/user-attachments/assets/c1ea5fdf-cb19-4d28-8518-411e7f1360ef)

## **index.html**
![image](https://github.com/user-attachments/assets/86094275-7dd6-4eb4-9c53-96b22daf8a79)

網頁主頁面:
顯示現金庫存、現金更動紀錄(含刪除按鈕功能)、股票庫存(含刪除功能)、股票庫存占比圖、資產比例占比圖



