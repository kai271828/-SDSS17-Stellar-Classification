# SDSS17-Stellar-Classification
## 專題實作目的
Stellar Classification Dataset - SDSS17 資料集紀錄 10 萬筆史隆數位巡天計畫觀測到的天體數據，包括光譜數據、紅移值等，而 Kaggle 上的一個社群競賽 (https://www.kaggle.com/c/nytfug) 以這個資料集作為比賽題目，分出 6 萬筆作為訓練資料，這個專題的目的是通過這些資料建立分類的資料探勘的模型，能夠根據給定的特徵區分出恆星、星系、類星體這三種星體。
## 採用 Data Mining 模組
分類器我類神經網路(ANN)來實作，使用的模組有 scikit-learn 和 Pytorch，其中 scikit-learn 主要使用 MLPClassifier 這個函式來快速建立簡易的 ANN 分類模型，而 Pytorch 則用來實作我自己的 ANN，能更有彈性的調整整個模型架構。
## 程式/環境設定&執行方式說明
執行 scikit-learn 程式碼的環境以 Jupyter Notebook 為主，Pytorch 的環境則使用了 Google Colab，若不使用 Google Colab，可以不執行程式中 Load Google Drive 的區塊。另外。實際執行時要將 Dataloader 區塊中 pd.read_csv 函式的路徑參數修改。
