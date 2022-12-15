
# 簡介

本 project 嘗試便用 Trime 重現港式中英混合輸入鍵盤。而家仲係好初步既階段，暫只支援倉頡。


# 安裝步驟

1. 安裝 [Trime 3.2.8](https://github.com/osfans/trime/releases) (新的應該也可以，未試)
2. Copy 所有檔案到 `你的Android/rime` 入面。
3. 開啟「同文輸入法」，按「部署」，
4. 再揀方案，要同時揀 "cangjie5_tc" & "hk_mixed_cangjie5" (唔肯定)
5. 第一次開有機會 load 好耐好耐 (5 分鐘或以上)

# 修改 Tips

* 基本上只需要改  `trime.custom.yaml` 和 `hk_mixed_cangjie5.custom.yaml`
* 請參考 [Trime Wiki](https://github.com/osfans/trime/wiki/trime.yaml) 和
* 修改 `trime.custom.yaml` 後，記得到「同文輸入法」>「主題與配色」>「主題」>  「Trime」> 「確定」一次，以 apply 你的修改。
* 修改 `cangjie5_tc.custom.yaml` (輸入法)後，要按「部署」。
* 如果修改好似無反應，請到 /rime/build 下查看有沒有你新的改動。

# 問題

* 「語音輸入」出現沒有權限的話，請自行到 Android 設定給予相關權限。

# 鳴謝

* 項目：[RIME], [TRIME], [倉頡五代補完計劃](https://github.com/Jackchows/Cangjie5)

[RIME]: http://rime.im
[TRIME]: https://github.com/osfans/trime
