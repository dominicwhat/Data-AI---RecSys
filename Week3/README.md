# Week 3

# 專案目的
## 比較「Collaborative Filtering 」三種方法產生的結果。 

# 結果
## 預設
### User-based collaborative filtering: 0
### Item-based collaborative filtering: 0.0017
### 套件 surprise 實作 collaborative filtering: 0.0017

## 與rule-based方法混用
### User-based collaborative filtering: 0.1
### Item-based collaborative filtering: 0.0983
### 套件 surprise 實作 collaborative filtering: 0.1

# 推薦算法
## 預設
### User-based collaborative filtering
### Item-based collaborative filtering
### 套件 surprise 實作 collaborative filtering
## 與rule-based方法混用
### 由於本次三種算法與上次 content-based算法遇到一樣的問題(亦即 testing data的使用者在training data中的資料太少)，因此採用上次做法，與 rule-based方法(推薦testing data前一年同月份評價數top 10的商品) 混合使用，得到比預設算法較佳的結果。

# 結論
## 這項專案希望藉由實作User-based collaborative filtering、 Item-based collaborative filtering 、 套件 surprise 實作 collaborative filtering，比較三種方法的推薦效果。
## 惟因資料的先天限制上遇到與上次作業類似的問題(即 testing data的使用者在training data中的資料太少 )，因此預設的推薦效果不甚理想。
## 解決辦法是同上次作業，針對testing data中沒辦法用三種推薦算法的使用者，用以前作業的rule-based方法(推薦testing data前一年同月份評價數top 10的商品)，得到比一開始好一點的推薦效果。
## 三種推薦方法，在預設及與rule-based混用的情況下，其表現似乎沒有太大的不同，推測是因為testing data的使用者在training data中的資料太少，導致三種算法均沒辦法呈現其原有的表現。  
