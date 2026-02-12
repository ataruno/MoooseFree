# firmwareの概要  
## MoooseFree_firmware_110  
### ロータリーエンコーダの感度を調整。  
左手側の大きなノブがついたロータリーエンコーダをtap-ms=<16>に変更  
右手側はtap-ms=<20>のまま。  

### 電波強度を高くする設定を反映  
CONFIG_BT_CTLR_TX_PWR_PLUS_8=yを設定。  
zmkの公式ドキュメントの"Unreliable/Weak Connection"を参照。  
https://zmk.dev/docs/troubleshooting/connection-issues  

