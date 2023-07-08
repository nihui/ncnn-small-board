# ncnn 小板子

ncnn is a high-performance neural network inference framework.

See https://github.com/Tencent/ncnn for more info about ncnn.

* The benchmark score is the inference time, **less is better**.
* Runs on all cpu big cores or vulkan, and fp16 arithmetic is enabled if supported.
* Table contents are ordered by mobilenet.
* Rock5B data from https://forum.radxa.com/t/rock5-android12-bringup-status-update/8506/17

|small-board|image|spec|squeezenet|mobilenet|shufflenet|
|---|---|---|---|---|---|
|NVIDIA Jetson AGX Orin|![](/images/jetsonagxorin.jpg)|Ampere 1.3GHz x 2048<br /><br />Tensor Core x 64|2.13|2.03|2.57|
|NVIDIA Jetson AGX Orin|![](/images/jetsonagxorin.jpg)|A78AE 2.2GHz x 12|3.50|3.49|5.08|
|Radxa Rock5B|![](/images/rock5b.jpg)|RK3588<br /><br />A76 2.4GHz x 4<br />A55 1.8GHz x 4|4.21|5.75|4.39|
|ZYSJ RK3588| |ARM Mali-G610|7.09|9.16|5.88|
|ZYSJ RK3588| |RK3588<br /><br />A76 2.4GHz x 4<br />A55 1.8GHz x 4|7.57|11.01|7.95|
|NVIDIA Jetson Nano|![](/images/jetsonnano.jpg)|Maxwell 921MHz x 128|9.03|15.39|10.61|
|Khadas VIM4|![](/images/vim4.jpg)|ARM Mali-G52<br /><br />800MHz x MP8(8EE)|12.77|20.17|12.81|
|Unisoc Tiger T710|![](/images/unisoct710.jpg)|Unisoc Tiger T710<br /><br />A75 1.82GHz x 4<br />A55 1.82GHz x 4|16.25|20.31|10.59|
|Khadas VIM3|![](/images/vim3.jpg)|ARM Mali-G52<br /><br />800MHz x MP4(6EE)|19.54|31.62|17.91|
|Radxa Rock3A|![](/images/rock3a.jpg)|RK3568<br /><br />A55 2.0GHz x 4|29.52|34.47|23.62|
|NanoPi M4|![](/images/nanopim4.jpg)|ARM Mali-T864|24.57|35.86|33.90|
|Radxa RockPi X|![](/images/rockpix.jpg)|Intel HD Graphics (Cherry Trail) 500 MHz|29.91|36.41|24.54|
|Khadas VIM4|![](/images/vim4.jpg)|A311D2<br /><br />A73 2.2GHz x 4<br />A53 2.0GHz x 2|24.27|37.65|19.79|
|NVIDIA Jetson Nano|![](/images/jetsonnano.jpg)|A57 1.43GHz x 4|28.55|40.25|19.44|
|Khadas VIM3|![](/images/vim3.jpg)|A311D<br /><br />A73 2.2GHz x 4<br />A53 1.8GHz x 2|30.98|42.57|21.62|
|NanoPi Fire3|![](/images/nanopifire3.jpg)|S5P6818<br /><br />A53 1.4GHz x 8|41.81|52.33|33.54|
|Odroid XU4|![](/images/odroidxu4.jpg)|Exynos 5422<br /><br />A15 2GHz x 4<br />A7 1.3GHz x 4|41.42|55.91|23.12|
|Debix Model A|![](/images/debixmodela.jpg)|i.MX8M Plus<br /><br />A53 1.6GHz x 4|44.60|59.50|30.34|
|Raspberry Pi 4B|![](/images/rasp4b.jpg)|BCM2711B0<br /><br />A72 1.5GHz x 4|46.28|60.74|32.91|
|Tinker Board S R2.0|![](/images/tinkersr2.jpg)|ARM Mali-T764|41.78|62.67|56.83|
|NanoPi M4|![](/images/nanopim4.jpg)|RK3399<br /><br />A72 1.8GHz x 2<br />A53 1.5GHz x 4|43.73|64.28|27.43|
|BeagleBone AI 64|![](/images/bbai64.jpg)|TDA4VM<br /><br />A72 2.0GHz x 2|42.23|65.78|29.97|
|Radxa Zero|![](/images/radxazero.jpg)|S905Y2<br /><br />A53 1.8GHz x 4|51.92|66.12|37.15|
|NanoPi K2|![](/images/nanopik2.jpg)|S905<br /><br />A53 1.5GHz x 4|56.96|75.25|38.70|
|Radxa RockPi X|![](/images/rockpix.jpg)|Atom x5-Z8350<br /><br />x86-64 1.92 GHz x 4|50.22|80.12|37.96|
|NanoPi R2S|![](/images/nanopir2s.jpg)|RK3328<br /><br />A53 1.3GHz x 4|62.20|82.88|52.34|
|Tinker Board S R2.0|![](/images/tinkersr2.jpg)|RK3288CGW<br /><br />A17 1.8GHz x 4|56.32|83.56|35.96|
|EAIDK 310|![](/images/eaidk310.jpg)|RK3228H<br /><br />A53 1.3GHz x 4|68.97|90.87|48.22|
|Radxa Zero|![](/images/radxazero.jpg)|ARM Mali-G31 850 MHz x 2|55.29|98.45|52.24|
|Raspberry Pi 3B+|![](/images/rasp3b.jpg)|BCM2837B0<br /><br />A53 1.4GHz x 4|84.74|107.84|58.38|
|Raspberry Pi Zero 2W|![](/images/raspz2.jpg)|BCM2710A1<br /><br />A53 1.0GHz x 4|119.52|162.60|72.72|
|EASY EAI Nano|![](/images/easyeainano.jpg)|RV1126<br /><br />A7 1.5GHz x 4|105.16|163.82|68.79|
|StarFive VisionFive V2|![](/images/visionfivev2.jpg)|SiFive’s U74<br /><br />RV64GFC 1.5GHz x 4|150.07|256.21|91.14|
|RVB-ICE|![](/images/ice.jpg)|T-Head C910<br /><br />RV64GC 1.2GHz x 2|161.10|274.39|118.61|
|Loongson Pie Lite|![](/images/ls2k.jpg)|Loongson 2K1000<br /><br />GS264 1.0GHz x 2|185.28|276.03|124.39|
|Ingenic X2000||Ingenic X2000<br /><br />XBurst2 1.2GHz x 2|175.99|282.25|118.4|
|Raspberry Pi 2B|![](/images/rasp2b.jpg)|BCM2836<br /><br />A7 900MHz x 4|179.50|296.97|132.49|
|Banana Pi M2 Zero 2|![](/images/bananaz2.jpg)|AllWinner H2+<br /><br />A7 1.2GHz x 4|218.73|303.92|138.43|
|Raspberry Pi 4B|![](/images/rasp4b.jpg)|Broadcom VideoCore VI|286.71|365.04|162.14|
|PICO-PI-IMX7|![](/images/pico.jpg)|i.MX7D<br /><br />A7 1.0GHz x 2|220.10|366.92|137.02|
|Microphase Z7-Lite|![](/images/z7lite.jpg)|XC7Z020CLG400<br /><br />A9 766MHz x 2|389.18|623.71|212.20|
|MangoPI MQ-Pro|![](/images/mq-pro.jpg)|D1 C906<br /><br />RV64GCV 1GHz x 1|385.21|691.47|487.67|
|NeZha D1|![](/images/nezhad1.jpg)|D1 C906<br /><br />RV64GCV 1GHz x 1|396.18|727.97|495.87|
|StarFive VisionFive V1|![](/images/visionfivev1.jpg)|SiFive’s U74<br /><br />RV64GFC 1.5GHz x 2|609.41|993.87|358.98|
|Raspberry Pi B+|![](/images/raspbp.jpg)|ARM1176JZF-S<br /><br />700MHz x 1|4646.13|8239.03|2141.68|
