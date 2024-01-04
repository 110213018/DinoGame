# 尋找顏⾊的⼩恐⿓
## 動機：
⼩恐⿓因為linux考不及格，被⽣氣的助教們變成灰⾊的了！！⼩恐⿓聽說只要穿越了
⼤森林，抵達魔法洞⽳，就可以找回顏⾊，快來幫助⼩恐⿓找回顏⾊吧！
## 功能：
有⼀台復古式遊戲台，按下巨型ENTER鍵後，即可開始遊玩遊戲。分數是以存活時間計算，一旦撞到障礙物之後分數會歸零，按按鍵就可以重新遊玩。開始遊玩後，如果每撐過一段時間，燈就會亮⼀種顏⾊，成功撐過最終目標時間的話，燈就會三個都亮起來，代表小恐龍都把顏色找回來了~
## 硬體設備：
- Raspberry pi 3
- 麵包板專⽤線
- 麵包板
- 巨型ENTER鍵
- 杜邦線
- ~~IR感測器(180度)~~
- led燈
- ~~小型按鍵~~
- register
- 紙箱
- moli捐贈的電腦螢幕
## 軟體
- python
- pygame
## 前置下載
- pygame
- python
## 執行過程
- 程式碼
  - dino.py：恐龍遊戲
  - redLED.py：模擬紅色led燈亮起
  - greenLED.py：模擬綠色led燈亮起
  - yellowLED.py：模擬黃色led燈亮起
  - Button.py：模擬開始按鈕 -> 無法套用
- 硬體準備
  - raspberry pi環境組裝
  - 遊戲機台組裝
  - 紅外線感應裝置 -> fail
  - LED燈裝置
  - 遊戲開始按鈕 ->從小按鈕變成巨型ENTER鍵(感謝熱心助教贊助)
## DinoGame START！
- 執行程式碼：python dino.py
- 按下巨型ENTER鍵!!
## 心得回饋&遇到的困難
1. raspberry pi環境組裝
因為在製作過程中，raspberry pi疑似因為過熱燒壞了，所以再重新設定raspberry pi上花了很多的心力跟時間。
2. 遊戲機台組裝
因為螢幕一直更換，所以重做了3次，好開心。
3. 紅外線感應裝置
我們使用的是型號為MH-B的IR感測器，疑似因為放了長時間受潮導致故障，不知道為甚麼接收器一直接受到來源不明的訊號，後續有嘗試上網搜尋、撰寫程式碼，但就算程式碼成功編譯結果一樣無法正常運作(都是紅外線有被東西擋住造成反射)，最後經過長時間的奮鬥後不得已宣告放棄。
4. LED燈裝置
從零開始學習接這些電路，發現這些東西會因為許多細小的因素被影響，像按鈕插入麵包版的深度或濕度等等~ 所以偶爾換個環境做也許會有新的發現!
5. dinoGame遊戲
原本是用ursino開發遊戲，但是當要在樹莓派上運行時，跳出提示說要安裝Panda3d，但在安裝上有困難，所以最後決定用pygame的形式表現出小恐龍遊戲。再加上，原本要外接的迷你螢幕，因為性能不足，無法顯示遊戲，所以最後決定用HDMI線的方式連接到性能較完善的電腦螢幕，最後就成功了~！！
6. 小按鈕裝置
  在麵包版上新增一個按鈕，功能為按下後，觸發遊戲開始。但是不知道怎麼讓dino.py知道這個鍵，所以最後用大型ENTER鍵代替小按鈕裝置變成開始鈕。
8. 程式碼整合
大家一起討稐~

## 工作分配
- 許湘蝶：紅外線感測裝置、LED燈裝置、創意發想、小按鈕裝置
- 楊于葳：LED燈裝置、材料購買、創意發想、小按鈕裝置
- 陳宣閔：dinoGame、撰寫README、創意發想
- 劉仁傑：遊戲機台組裝、材料購買
- 許家維：dcard宣傳
- 感謝Josh、蓬萊人偶等熱心助教的指導~^^
## 善用所學
linux系統指令、python、raspberry pi、os、高等物理
## 參考資料
- 遊戲軟體參考：https://github.com/maxontech/chrome-dinosaur
- 紅外線感測參考：https://youtu.be/7i0dvQGM-Zk?si=t10epjFb-RD5S5_6
- led裝置參考：https://www.youtube.com/watch?v=kfb34fn9zpo&t=276s
