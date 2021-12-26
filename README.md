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
