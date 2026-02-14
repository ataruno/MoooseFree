# firmwareの概要  
## MoooseFree_firmware_120  
### 110のバグ修正版  
音量設定が動作するように一部修正しました。  
CONFIG_EC11_TRIGGER_OWN_THREADからCONFIG_EC11_TRIGGER_GLOBAL_THREADに戻す  

## MoooseFree_firmware_110  
### 追記
110はバグあり。  
デフォルト以外のレイヤーでの音量設定がうまく動作しない  
最新の114をお使いください。  

### ロータリーエンコーダの感度を調整。  
左手側の大きなノブがついたロータリーエンコーダをtap-ms=<16>に変更  
右手側はtap-ms=<20>のまま。  
※注意：左手側のエンコーダをかなり高速に回すと暴走(=スクロールしっぱなし)します。  
  両手ともに電源をOFFして、再度電源ONしてください。  
  また、過度に高速で回しすぎないようお願いします。  
  上記の設定値変更で低減するよう改善はできました。  

### 電波強度を高くする設定を反映  
CONFIG_BT_CTLR_TX_PWR_PLUS_8=yを設定。  
zmkの公式ドキュメントの"Unreliable/Weak Connection"を参照。  
https://zmk.dev/docs/troubleshooting/connection-issues  

