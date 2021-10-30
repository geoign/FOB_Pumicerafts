# 概要
福徳岡ノ場2021年噴火は200-数千km2にわたって海に広がる複数の軽石いかだを形成した。
本データセットは特定時間における個々の軽石いかだの広がりを衛星写真からトレースしたshapefileである。

# お願い
本データは災害状態にあることに鑑みて早期公開するもので、より詳細な記載を行った論文は準備中である。
2021/10/30現在、本データを分析し論文を投稿するのであれば、コンフリクトを防ぐために連絡してほしい。
連絡先: f.ikegami_at_gmail.com あるいは geoign@Twitter

# データ構造
時間は年月日T時刻Zで表記してあるとおり、すべてUTCである。
雲に隠された部分は、内挿できる場合は直線で内挿し、できない場合は直線で切り落としている。

## FOB2021_PumiceDrift2_WGS84.shp
8/13 - 9/18までの期間における、衛星写真で判別可能なすべての軽石ラフトをトレースしたデータである。
トレース元の衛星写真は解像度数百m程度の、NASA MODIS衛星群 (Terra, Aqua, Suomi)、およびESA Sentinel-3衛星を用いた。
台風16号Mindulleの接近により識別困難となるまで、40個の衛星写真から累計778個の軽石ラフトを識別した。
更新は終了しているが、今後小規模な修正を行う可能性がある。

## FOB2021_PumiceDrift4_WGS84.shp
10/9以降の期間における、衛星写真において多量のラフトが密集していると考えられる範囲を矩形で囲ったデータである。
トレース元の衛星写真は高解像度なESA Sentinel-2、NASA Landsat-8、そして補助的にSentinel-3も用いた。
10/30現在逐次更新しており、既存のデータも大幅に修正する可能性がある。
