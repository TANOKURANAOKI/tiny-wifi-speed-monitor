# tiny-wifi-speed-monitor
Raspberry Pi Pico W で検知したWifiの速度が一定値を下回った時にLEDを点灯させるシステムです。

# 開発の概要
## 背景
2025年1月現在の住まいではホームWi-Fiを利用しているが、ダウンロード速度が最も遅いときで2Kと非常に遅い回線速度となっている。

## 実装内容
実態の検証のため、Raspberry Pi Pico Wを使い以下の機能を実現する。
１．一定の回線速度を下回った時に付属のLEDライトを利用し、いわゆるLチカと呼ばれるLEDの点灯を行い、回線速度の低下を目視させる。
２．Lチカの期間に応じて、回線の低下のタイミングを検知し、どの時間帯の場合回線速度が下がる傾向にあるかを分析する。
