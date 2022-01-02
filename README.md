# Week 1

# 專案目的
## 實作「rule-based」的推薦系統

# 結果
## 使用四種方法 隨機推薦 score:0.014, 推薦評價次數topK商品:0.083, 推薦2018年8月評價次數topK商品: 0.154, 推薦2017年9月評價次數topK商品: 0.1

# 推薦算法

### 隨機推薦: 隨機推薦training data的K個商品

### 推薦評價次數topK商品: 推薦training data最多人評價的K個商品

### 推薦2018年8月評價次數topK商品: 推薦2018年8月training data最多人評價的K個商品

### 推薦2017年9月評價次數topK商品: 推薦2017年9月training data最多人評價的K個商品

# 結論
## 在考慮時間性後，推薦前一個月的training data評價次數topK商品比考慮前一年同月份training data評價次數topK商品的準確率高。惟兩者均比不考慮時間性及隨機推薦的方法來得好

# Week 2

# 專案目的
## 實作「Content-based Filtering」的推薦系統

# 結果
## 預設Content-based score:0, Content-based+rule-bases score: 0.097

# 推薦算法

### 預設Content-based: 對testing data的每個使用者，使用Content-based 算法做推薦

### Content-based+rule-bases: 除了使用Content-based 算法做推薦，針對testing data沒辦法用content-based算法做推薦的使用者，改使用Week1 rule-based的算法(推薦testing data前一年同月份評價數top 10的商品)做推薦 

# 結論
## 這項專案希望藉由content-based的演算法提供部分使用者的推薦商品，惟在testing data的使用者在training data中的資料太少，較難對針對每個 testing data 的使用者做content-based的推薦。 因此整體推薦的效果並不理想。解決辦法是針對testing data中沒辦法用content-based推薦算法的使用者，用上次作業的rule-based方法，推薦testing data前一年同月份評價數top 10的商品，得到比一開始好一點的推薦效果
