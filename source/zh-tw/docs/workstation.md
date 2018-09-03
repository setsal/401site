title: Workstation
---

## 工作站
目前系上提供三台 FreeBSD 工作站與兩台 Linux 工作站：
- **FreeBSD**
    - csie0.cs.ccu.edu.tw
    - csie1.cs.ccu.edu.tw
    - csie2.cs.ccu.edu.tw

- **Linux**
    - linux.cs.ccu.edu.tw
    - mcore8.cs.ccu.edu.tw

----

## 使用者帳號

### 本系生
- 本系生的帳號資訊會在入學後以紙本告知。
- 五台工作站的帳號與家目錄內的資料皆是共通的。
- 只要依據需求及工作站負載狀況，選擇合適的機器來使用。

### 外系生
- 外系生修習資工系課程時，可在該學期至資工系系辦申請帳號。
- 詳細說明請參閱 [外系生帳號申請](./external.html) 。

----

## 連線
### SSH
- 請以任何支援 SSH protocol version 2 的程式來登入工作站。
    - Windows 使用者可使用如 PuTTY, PieTTY, MobaXterm, ...。
    - Unix-like 使用者可以使用 OpenSSH, Dropbear, ...。
<br/>

- 登入方式：
``` Shell-Script
ssh 帳號名稱@工作站位址
```
- 範例：
``` Shell-Script
ssh user@csie1.cs.ccu.edu.tw
```
### FTP
- 建議使用 SFTP 傳輸檔案以增加安全性。
- 目前支援 FTP 傳輸檔案的工作站有 csie0.cs 和 csie1.cs。

### SFTP
- 所有工作站皆有支援 SFTP 協定。

----

## Quota 
系上儲存空間有限，故實施以下限制：
- 家目錄容量限制 ( ~/ ) :
    - 大學部在校生：10 GB
    - 碩士班在校生： 3 GB
    - 畢業大學部、碩士班校友：1 GB


- Quota 限制有緩衝 0.5 GB，即在超過 quota，但未超出 0.5 GB 時，有三日緩衝時間，如超過上限或超過三日緩衝時間，將無法再進行資料寫入。


- 查看目前用量與 quota 限制：
    - FreeBSD
``` Shell-Script
    quota -h
```
    - Linux
``` Shell-Script
    quota -s
```
