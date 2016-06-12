#SoftwareStudioAssignment8
分成兩部分解釋:Client端與Server端  
Client端: 總共有三個page，分別是輸入IP、計算與結果的頁面。在輸入IP的頁面，會用String變數存取輸入的IP，在計算的
operator按下後，用IP跟設定好的port 去連線。當連線上之後，便會將答案用write函式傳送到server端，最後結果兩邊都會
顯示。    
Server端: 先建立一個JFrame，並用JTextArea顯示可以換行的text，在連線後便可以用setText函式將結果顯現出來。  
  
遇到的困難: 因為看Spec沒有看仔細的緣故，在連線的時候一直無法連上，後來上網查詢錯誤代碼才發現是在  
AndroidManifest.xml裡忘記加<uses­permission android:name="android.permission.INTERNET"/>這一行。在沒看到錯誤代  
碼之前浪費蠻多時間重複trace code的。
