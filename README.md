# ncnn 小板子

ncnn is a high-performance neural network inference framework.

See https://github.com/Tencent/ncnn for more info about ncnn.

* The benchmark score is the inference time, **less is better**.
* Runs on all cpu big cores or vulkan, and fp16 arithmetic is enabled if supported.
* Table contents are ordered by mobilenet.
* Rock5B data from https://forum.radxa.com/t/rock5-android12-bringup-status-update/8506/17

|small-board|image|spec|squeezenet|mobilenet|shufflenet|
|---|---|---|---|---|---|
|Radxa Rock5B|![](/images/rock5b.jpg)|RK3588<br /><br />A76 2.4GHz x 4<br />A55 1.8GHz x 4|9.38|11.97|8.02|
|NVIDIA Jetson Nano|![](/images/jetsonnano.jpg)|Maxwell 921MHz x 128|12.00|16.03|14.23|
|Unisoc Tiger T710|![](/images/unisoct710.jpg)|Unisoc Tiger T710<br /><br />A75 1.82GHz x 4<br />A55 1.82GHz x 4|16.25|20.31|10.59|
|Khadas VIM3|![](/images/vim3.jpg)|ARM Mali-G52|19.54|31.62|17.91|
|Radxa Rock3A|![](/images/rock3a.jpg)|RK3568<br /><br />A55 2.0GHz x 4|29.52|34.47|23.62|
|NanoPi M4|![](/images/nanopim4.jpg)|ARM Mali-T864|24.57|35.86|33.90|
|Radxa RockPi X|![](/images/rockpix.jpg)|Intel HD Graphics (Cherry Trail) 500 MHz|29.91|36.41|24.54|
|NVIDIA Jetson Nano|![](/images/jetsonnano.jpg)|A57 1.43GHz x 4|30.03|41.74|21.07|
|Khadas VIM3|![](/images/vim3.jpg)|A311D<br /><br />A73 2.2GHz x 4<br />A53 1.8GHz x 2|30.98|42.57|21.62|
|Tinker Board S R2.0|![](/images/tinkersr2.jpg)|ARM Mali-T764|41.78|62.67|56.83|
|NanoPi M4|![](/images/nanopim4.jpg)|RK3399<br /><br />A72 1.8GHz x 2<br />A53 1.5GHz x 4|43.73|64.28|27.43|
|Radxa Zero|![](/images/radxazero.jpg)|S905Y2<br /><br />A53 1.8GHz x 4|51.92|66.12|37.15|
|Raspberry Pi 4B|![](/images/rasp4b.jpg)|BCM2711B0<br /><br />A72 1.5GHz x 4|58.38|71.59|37.93|
|Radxa RockPi X|![](/images/rockpix.jpg)|Atom x5-Z8350<br /><br />x86-64 1.92 GHz x 4|50.22|80.12|37.96|
|NanoPi R2S|![](/images/nanopir2s.jpg)|RK3328<br /><br />A53 1.3GHz x 4|62.20|82.88|52.34|
|Tinker Board S R2.0|![](/images/tinkersr2.jpg)|RK3288CGW<br /><br />A17 1.8GHz x 4|56.32|83.56|35.96|
|EAIDK 310|![](/images/eaidk310.jpg)|RK3228H<br /><br />A53 1.3GHz x 4|68.97|90.87|48.22|
|Radxa Zero|![](/images/radxazero.jpg)|ARM Mali-G31 850 MHz x 2|55.29|98.45|52.24|
|Raspberry Pi 3B+|![](/images/rasp3b.jpg)|BCM2837B0<br /><br />A53 1.4GHz x 4|93.48|111.72|63.71|
|Raspberry Pi Zero 2W|![](/images/raspz2.jpg)|BCM2710A1<br /><br />A53 1.0GHz x 4|119.52|162.60|72.72|
|Loongson Pie Lite|![](/images/ls2k.jpg)|Loongson 2K1000<br /><br />GS264 1.0GHz x 2|185.28|276.03|124.39|
|Banana Pi M2 Zero 2|![](/images/bananaz2.jpg)|AllWinner H2+<br /><br />A7 1.2GHz x 4|230.97|327.65|147.97|
|PICO-PI-IMX7|![](/images/pico.jpg)|i.MX7D<br /><br />A7 1.0GHz x 2|220.10|366.92|137.02|
|Raspberry Pi 2B|![](/images/rasp2b.jpg)|BCM2836<br /><br />A7 900MHz x 4|231.20|363.92|141.96|
|Microphase Z7-Lite|![](/images/z7lite.jpg)|XC7Z020CLG400<br /><br />A9 766MHz x 2|389.18|623.71|212.20|
|NeZha D1|![](/images/nezhad1.jpg)|D1 C906<br /><br />RV64GCV 1GHz x 1|408.03|731.92|466.21|
