title: 外系生
---
## 內容及相關規定

+ 提供修習資工系開設相關課程的外系生，練習程式或繳交作業的平台。
+ 申請之帳號使用以一個學期為限，帳號將於學期結束後刪除。請自行備份工作站上之個人資料，帳號刪除後，將不負責個人資料之保存。
+ 申請者請確實遵守電算中心之「教育部校園網路使用規範」和「智慧財產權」等相關法令。
+ 外系生帳號和本系生帳號之權限不盡相同，如有特殊需要，請告知系統管理員。

## 申請流程

### 個別申請

1. 請下載填寫本申請單：[外系生帳號個人申請單.doc](doc/CS_applications.doc)
2. 請詳閱申請單上之相關規定。
3. 填寫完畢後，請交至資工系辦。
4. SA 於完成審核後，會以 E-mail 通知申請者結果以及相關的訊息。

### 統一申請

1. 請課程助教下載並協助同學填寫本申請單：[外系生帳號統一申請單.doc](doc/CS_applications_group.doc)
2. 請詳閱申請單上之相關規定。
3. 填寫完畢後，請交至資工系辦。
4. SA 於完成審核後，會以 E-mail 個別通知申請者結果以及相關的訊息。

## 外系生工作站資訊

+ 位址：csie2.cs.ccu.edu.tw
+ 連線：請以任何支援 SSH protocol version 2 的程式來登入工作站。
    + Windows 使用者可使用 PuTTY, PieTTY, MobaXterm, ...。
    + Unix-like 使用者可使用 OpenSSH, Dropbear, ...。


+ SSH 登入方式
```bash
ssh 帳號名稱@csie2.cs.ccu.edu.tw
```

+ 更改密碼：連線至工作站後輸入指令
```bash
passwd
```
+ 忘記密碼
請本人親持學生證至資工系辦申請補發新密碼。


+ FTP 檔案傳輸
請使用支援 SFTP 協定之 FTP client 軟體（如 FileZilla）來存取 FTP 服務，連線時選擇 SFTP 協定，以增加網路傳輸的安全性。


+ Web Page
請連線至工作站，並到自己的家目錄下建立 WWW 目錄。
```
mkdir WWW
```
    + 首頁檔名必需為 index.html, index.php, 或 index.shtml 。
    + 使用者的 URL 為 `http://www2.cs.ccu.edu.tw/~帳號名稱/`
