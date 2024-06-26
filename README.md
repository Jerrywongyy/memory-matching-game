# 如何製作memory matching game？
# 背景：
- 當2張卡抽出相同的圖案時就是成功的第一步
- 而把所有卡抽出後才是成功結束整個遊戲
# 1.HTML架構：
- 在創建網頁標題為memory-matching-game
- 在網頁中添加主要區塊，要有4x4的可點擊網格
- 記住加入header（標題）和footer（頁腳）
# 2.CSS樣式：
- 為所有元素設定指定字體
- 為網格設定紅色背景和點擊指示符
- 網格區塊居中顯示，每個網格項目平均分佈
- 設定區塊裏的圖案/emo😀
- 遊戲版面要置中對齊
# 3.Javascript邏輯：
## 3.1初始化：將變數matchCount預設為0
- 一開始，玩家會看見memory matching game 的版面。玩家要按下區塊=（抽卡）
- 不同區塊的圖案要隨機放置
- 當玩家隨機點擊第一個跟第二個區塊時，區塊會顯示圖案
## 3.2檢測兩個區塊的圖案的條件：
### 當對的時候：
- 如果區塊的圖案不相同，第一個跟第二個區塊要反轉。並且繼續遊戲。🈳
- 變數matchCount要減2
### 當錯的時候：
- 如果區塊的圖案相同，第一個跟第二個區塊不用反轉。並且繼續遊戲。🈯
- 變數matchCount要繼續加上去
- 同時設一個變數為match count去記錄玩家按下不同區塊的次數
## 3.3當遊戲結束時的條件：
- 當玩家把所有卡全部揭開後，必須要顯示遊戲結束，然後生成一個重玩遊戲的按鈕，還原一開始memory matching game 的版面。🔃
- 當變數clickCount大於或等於16，必須要中止遊戲進行‼️
## 另外的event listener幫助
- 加入event listener 監聽器來處理玩家的點擊動作。
# 4.進階功能
### 單人的玩法：
- 新增另一個變數叫clickResult:這個變數不同於clickCount,它是計算玩家的點擊總次數。
- 新增計時器令遊戲提高難度。
- 在區塊的圖案加入一個好處：例如:新增加時的圖案，令玩家有時間盡快完成遊戲。
- 設置玩家在遊戲開始後有四個機會=（四個生命值），如果區塊的圖案不相同的次數超過4次，遊戲結束。
### 雙人的玩法：
#### 新增計分器:
- 當其中一個玩家隨機點擊第一個跟第二個區塊的圖案時是相同，並向那位玩家加分。
- 當其中一個玩家隨機點擊第一個跟第二個區塊的圖案時是不相同，並向那位玩家扣分。
### final presentation
- https://docs.google.com/presentation/d/1-7rkhFMwbymeWRgw8kOvIHMvCk6pu8oF276IkNOCdgs/edit?usp=sharing
### final memory matching game
- https://replit.com/@WONG-YAT-YIYAT/Instagram-1#index.html
