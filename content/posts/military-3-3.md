---
title: "當兵必裝的國軍 MDM 簡介"
date: 2022-01-17
draft: false
categories: "Military"
tags: 
 - "Military"
---

簡單來說就是把手機的相機、藍牙、定位、熱點給停用，避免有人亂來造成軍機外洩

<!--more-->

本文以 iOS 為主，為了當兵裝 MDM 我還特地收一隻 iPhone 6s。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211187&authkey=%21AAqHO8eG2TZe3NU&width=2250&height=1334)

# 關於安裝

本文撰寫於 2022/01，目前已知有兩種安裝方式，一種是最原本的「描述檔」，另一種為「監管模式」，各單位採用的安裝模式都不同，若是監管模式的話會需要重置 iPhone，別問為什麼，蘋果文件就是這樣寫。

我在大內服役，採用描述檔的方式，撥交到外單位的弟兄有幾位要重裝，切換為監管模式，所以安裝方式視單位而定。

安裝會連到 `192.168.2.2/mdm/ios/tool.htm` 去做安裝，但我們連隊是班長幫我們安裝，所以詳細流程不清楚，隔壁兵器連是自行連線安裝，完成才拿去電腦那邊註冊。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211190&authkey=%21AOG_FuVnnwk4Dew&width=1500&height=1334)

# 上鎖與解鎖

每次進入營區前要給衛哨檢查，到連上後長官也會檢查一次。

## 上鎖

按下上鎖後會提示要求關閉「藍芽」及「定位」功能，需手動至設定內關閉，關閉後回到 APP 再次點擊上鎖即會開啟 Safari 並連線至 `127.0.0.1:6057/IililIloO0O0.mobileconfig` 下載上鎖用的描述檔，下載後須至設定中自行安裝，安裝後回到 APP 就會出現「已上鎖」。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211192&authkey=%21APgGOLUs7wc0cM4&width=1498&height=1334)
![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211191&authkey=%21AAcdqxrWSJJKCgk&width=1500&height=1334)

## 解鎖

有兩種解鎖模式，「快速」與「僅 GPS」。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211193&authkey=%21AAVcTHbStA8maRc&width=1500&height=1334)

- 快速

// TODO

- 僅 GPS

按下後會提示開啟定位服務，定位確認不在管制範圍內時會自動開啟 Safari 導向 `127.0.0.1:6057/IililIloO0O0.mobileconfig` 下載解鎖用描述檔，安裝後即可解鎖。但有時 Safari 會卡住無法下載，回到 MDM 就會顯示「拯救我的相機」(如圖最右邊)，按下後會重新下載一個描述檔，安裝後完成解鎖動作。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211194&authkey=%21ADcNn4QV6mzsmyI&width=3010&height=1334)

- 管制區內解鎖

離營區太近的狀況下解鎖就會這樣，別急著解鎖。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211195&authkey=%21AIq7ZjEhPysa-w4&width=1500&height=1334)

# 更新國軍 MDM

有兩位鄰兵於上鎖狀態更新沒出事，但我怕麻煩等放假才更新。按下「立即更新後」會導向安裝網頁，直接按「安裝 iOS MDM app」後就會自己裝了，超詭異。

若是分享網址，網址會長這樣: `https://update.mdm.mil.tw/imdm/install?t=87R92&o=1`

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211198&authkey=%21AGHMBqsKst4i7a0&width=3750&height=1334)

# 紀錄查詢

MDM 會記錄上鎖、解鎖、開機時間、MDM 啟動狀態…等事件，預設不會上傳。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211197&authkey=%21AIQr6z6d4WYE_CI&width=2250&height=1334)

# 側邊選單

沒錯，破 UI，都 2022 年了還會有狀態列看不清的問題。

![](https://onedrive.live.com/embed?resid=7AE5E29699A431DD%211196&authkey=%21AH65WfAeCdx_VMY&width=2304&height=1334)