
# 簡介

本 project 嘗試便用 Trime 重現港式中英混合輸入鍵盤。而家仲係好初步既階段，暫只支援倉頡。

# TODO 

- [ ] Fix Emoji
- [ ] 速成 （可成功，不過候選詞次序有問題）
- [ ] 英文反查

# 安裝步驟

1. 安裝 [Trime 3.2.8](https://github.com/osfans/trime/releases) (新的應該也可以，未試)
2. 開啟「同文輸入法」，允許所有權限
3. 下載此 repo 中的所有檔安，Copy 到 `內置儲存空間/rime` 入面。
3. 開啟「同文輸入法」，按「部署」(會 load 好耐好耐 (5 分鐘或以上))
4. 再揀「方案」，揀 "hk_mixed_cangjie5"
5. 第一次開有機會 load 好耐好耐 (5 分鐘或以上)

PS: 建議安裝 apk 後先開啟「同文輸入法」作設定。如未做第一次設定但已抄了檔案，做設定時畫面會 freeze 了沒有回應。如出現此情況，請繼續等。

# 修改 Tips

* 基本上只需要改  `trime.custom.yaml` 和 `hk_mixed_cangjie5.custom.yaml`
* 請參考 [Trime Wiki](https://github.com/osfans/trime/wiki/trime.yaml) 和 [Rime Customization Guide](https://github.com/rime/home/wiki/CustomizationGuide)
* 修改 `trime.custom.yaml` 後，記得到「同文輸入法」>「主題與配色」>「主題」>  「Trime」> 「確定」一次，以 apply 你的修改。
* 修改 `hk_mixed_cangjie5.custom.yaml` (輸入法)後，要按「部署」。
* 如果修改好似無反應，請到 `/rime/build` 下查看有沒有你新的改動。

# 常見問題

* 「語音輸入」出現沒有權限的話，請自行到 Android (設定 -> 應用程式)給予相關權限。
* 自定義詞庫中的，字詞與字碼中間必須為 tab (\t)，space 是沒有反應的。

# 鳴謝

* 項目：[RIME], [TRIME], [倉頡五代補完計劃], [如何優雅地在小狼毫使用倉頡輸入法], [RIME-Cantonese]

[RIME]: http://rime.im
[TRIME]: https://github.com/osfans/trime
[倉頡五代補完計劃]: https://github.com/Jackchows/Cangjie5
[RIME-Cantonese]: https://github.com/rime/rime-cantonese
[如何優雅地在小狼毫使用倉頡輸入法]: https://github.com/qingchen239/RimeCangjieInputConfiguration