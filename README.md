github: ziqinggao82-ux/1151VR-HW3-414262246-gzq
youtube:(電腦):https://youtu.be/9itwaIP64HM
(手機版):https://youtube.com/shorts/77SFCcIfR1s?feature=share
一、匯入素材
首先我把平台先切換為 Android，匯入白色圓形和三角形圖片，建立 Canvas把輪盤、指針、
按鈕、輸入框和結果文字放進場景中。
二、輪盤轉動
先用 6 個扇形組成輪盤，再用 Coroutine 做出轉動效果。
● 按下 SPIN ，輪盤就會開始旋轉。
● 設定減速曲線和隨機轉動角度，讓輪盤越轉越慢。
● 停下後利用角度除以每片扇形的角度，判斷指針指到哪個選項。
● 將結果顯示在畫面上。
三、新增和刪除選項功能
為了讓輪盤可以自訂內容，把扇形做成 SlicePrefab，用 List 儲存選項。
● 輸入文字按下新增按鈕，輪盤會自動生成對應數量的扇形。
● 點一下文字可以刪除該選項。
● 改用 HSV 自動配色，讓每個選項顏色都不一樣。
● 設定預設選項，並在選項刪光時提醒新增選項。
四、加入中文字型
因為 TextMeshPro 預設字型不支援中文，所以匯入 Noto Sans TC，套用到扇形文字、輸入
框、按鈕和結果文字，讓中文可以正常輸入。
五、加入音效
加入點擊聲、轉動聲和中獎聲，新增 Audio Source 控制播放。
● 新增、刪除和開始轉動時播放點擊聲。
● 轉動時播放轉動聲，讓轉動時間配合音檔長度。
● 得到結果時播放中獎聲。
六、輸出到手機
打開手機的開發者模式與和USB 偵錯，在 Build Profiles 確認平台為 Android，在 Player
Settings 設定 Package Name 和直式畫面，按下 Build And Run 輸出 APK。
