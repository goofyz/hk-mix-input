
# 簡介

本 project 嘗試便用 Trime 重現港式中英混合輸入鍵盤。

# 安裝步驟

1. 安裝 [Trime 3.2.16](https://github.com/osfans/trime/releases) (舊的不行啊)
2. 開啟「同文輸入法」，允許所有權限
3. 到「同文輸入法」 > 「鍵盤設定」> 「嵌入式編輯模式」> 揀 「輸入碼」，這樣打字時 default 會出英文。
3. 下載此 repo 中的[所有檔案](https://github.com/goofyz/hk-mix-input/archive/refs/heads/main.zip)，Copy 到 `內置儲存空間/rime` 入面。
3. 到「同文輸入法」 > 「主題與配色」 > 「主題」 > 「Trime」> 「確定」一次
3. 到「同文輸入法」 > 「方案」 > 揀 "hk_mixed_cangjie5/hk_mixed_quick" (會 load 好耐好耐 (5 分鐘或以上))
3. 按「部署」

PS: 抄了檔案後，開啟「同文輸入法」或部署時，會 load 好耐好耐 (5 分鐘或以上)
PS2: 建議安裝 apk 後先開啟「同文輸入法」作設定。如未做第一次設定但已抄了檔案，做設定時畫面會 freeze 了沒有回應。如出現此情況，請繼續等。

# 修改 Tips

- 基本上只需要改  `trime.custom.yaml` 和 `hk_mixed_cangjie5.custom.yaml`/`hk_mixed_quick.custom.yaml`
    - `trime.custom.yaml`: 修改外觀顏色和鍵盤設定
    - `hk_mixed_cangjie5.custom.yaml`/`hk_mixed_quick.custom.yaml`: 輸入法運作
- 請參考 [Trime Wiki](https://github.com/osfans/trime/wiki/trime.yaml) 和 [Rime Customization Guide](https://github.com/rime/home/wiki/CustomizationGuide)
- 修改 `trime.custom.yaml` 後，記得到「同文輸入法」>「主題與配色」>「主題」>  「Trime」> 「確定」一次，以 apply 你的修改。
- 修改 `hk_mixed_cangjie5.custom.yaml`/`hk_mixed_quick.custom.yaml` (輸入法)後，要按「部署」。
- 如果修改又 deploy 後，沒有反應，請到 `/rime/build` 下查看有沒有你新的改動。
- 有新詞語可新增到 `hk_mixed_input.custom.dict.yaml` ，注意字語和字碼之間是 tab 非 space。

# 常見問題

- 「語音輸入」出現「沒有權限」的話，請自行到 Android (設定 -> 應用程式)給予相關權限。
- 自定義詞庫中的，字詞與字碼中間必須為 tab (\t)，space 是沒有反應的。
- 如有問題可整個 `/rime/build` 刪除再重做一次。

# 鳴謝

- 項目：[RIME], [TRIME], [倉頡五代補完計劃], [如何優雅地在小狼毫使用倉頡輸入法], [RIME-Cantonese]

[RIME]: http://rime.im
[TRIME]: https://github.com/osfans/trime
[倉頡五代補完計劃]: https://github.com/Jackchows/Cangjie5
[RIME-Cantonese]: https://github.com/rime/rime-cantonese
[如何優雅地在小狼毫使用倉頡輸入法]: https://github.com/qingchen239/RimeCangjieInputConfiguration