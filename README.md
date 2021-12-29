# 概要
福徳岡ノ場2021年噴火は200-数千km2にわたって海に広がる複数の軽石いかだを形成した。
本データセットは特定時間における個々の軽石いかだの広がり(②④)および新規漂着日(③)を示したshapefileである。
10秒に動画化したもの: https://www.youtube.com/watch?v=-kI34Q69F1g

# お願い
本データは災害状態にあることに鑑みて早期公開するもので、より詳細な記載を行った論文は準備中である。
軽石の拡散シミュレーション試行時の比較用、あるいは衛星画像からの自動検出を試みる場合のクリッピングマスクとしての利用を想定している。
2021/12/29現在、本データを(比較ではなく)直接解析し論文を投稿するのであれば、コンフリクトを防ぐために連絡してほしい。
連絡先: 池上郁彦(タスマニア大学) f.ikegami_at_gmail.com あるいは geoign@Twitter

# データ構造
データセット②④の日付時刻はすべてUTCである。
雲に隠された部分は、内挿できる場合は直線で内挿し、できない場合は直線で切り落としている。
データセット③は日本時間での日付を記録している。

## データセット①：欠番

## データセット②：FOB2021_PumiceDrift2_WGS84.shp
8/13 - 9/23までの期間における、衛星画像で判別可能なすべての軽石いかだの外周をトレースしたデータである。
トレース元の衛星画像は解像度数百m程度の、NASA MODIS (Terra & Aqua)、NOAA Suomi NPP、およびESA Sentinel-3衛星を用いた。
台風16号Mindulleの接近により識別困難となるまで、40個の衛星写真から累計778個の軽石いかだを識別した。
更新は終了しているが、今後小規模な修正を行う可能性がある。

## データセット③：FOB2021_PumiceDrift3_WGS84.shp
特定の島・県・地域などへの軽石の新規漂着日を情報ソースとともに記録したデータである。多少だが情報を選別している。
ソースとして個人のSNS投稿URLを含んでいるが、くれぐれも迷惑がかからない＆失礼のない取り扱いを希望する。
更新は終了しているが、今後小規模な修正を行う可能性がある。

## データセット④：FOB2021_PumiceDrift4_WGS84.shp
9/19 - 11/11の期間における、衛星画像において多量の軽石いかだが密集していると考えられる範囲をおおまかに矩形で囲ったデータである。
トレース元の衛星画像は高解像度なESA Sentinel-2、NASA Landsat-8、低解像度なESA Sentinel-3およびNASA MODISが混在している。
軽石の拡散により識別困難となるまで、29個の衛星写真から累計312個の漂流範囲を識別した。
更新は終了しているが、今後小規模な修正を行う可能性がある。
