台鐵訂票規則
(一)針對每分鐘訂票超過 60 次身分證字號進行阻擋。
(二)異常訂票 IP 封鎖機制。
(三)驗證碼改為浮動碼（4~6 碼）。

要爬台鐵網站進行訂票一定要取得 session cookie，
直接爬訂票頁面會發生錯誤
爬時刻表網站需要 zLib 解壓縮

如何安裝
-----------------------------
step 1.
下載安裝OpenVPN 選擇Installer, Windows Vista and later
https://openvpn.net/index.php/open-source/downloads.html

並且到OpenVPN的安裝目錄   舉例 E:\OpenVPN\bin
右鍵點擊openvpn.exe ->內容 ->相容性頁籤 ->將"以系統管理員的身份執行此程式"勾選

Step2.
安裝Anaconda2  python2.7版本

Step3.
安裝以下package
conda install -c https://conda.binstar.org/menpo opencv
conda install -c anaconda requests=2.12.4

Step4.
安裝GCC編譯環境
指令:conda install mingw libpython
安裝Keras
Keras的相關設定請參考這篇
把backend改成theano
https://keras-cn.readthedocs.io/en/latest/getting_started/keras_windows/
