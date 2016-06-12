# SoftwareStudioAssignment8
分成兩部分解釋:Client端與Server端
Client:
  總共有三個page，分別是輸入IP、計算與結果的頁面。在輸入IP的頁面，會用String變數存取輸入的IP，在計算的operator按下後，用IP跟設定好的port
  去連線。當連線上之後，便會將答案用write函式傳送到server端，最後結果兩邊都會顯示。
Server端:
  先建立一個JFrame，並用JTextArea顯示可以換行的text，在連線後便可以用setText函式將結果顯現出來。
