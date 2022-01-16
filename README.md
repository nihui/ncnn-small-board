# ncnn 小板子

* The benchmark score is the inference time, less is better.
* Runs on all cpu big cores, and fp16 arithmetic is enabled if supported.
* Table contents are ordered by mobilenet.

|small-board|image|spec|squeezenet|mobilenet|shufflenet|
|---|---|---|---|---|---|
|Radxa Rock3A|![](/images/rock3a.jpg)|RK3568<br /><br />A55 2.0GHz x 4|29.52|34.47|23.62|
|NVIDIA Jetson Nano|![](/images/jetsonnano.jpg)|A57 1.43GHz x 4|35.56|38.39|34.39|
|Khadas VIM3|![](/images/vim3.jpg)|A311D<br /><br />A73 2.2GHz x 4<br />A53 1.8GHz x 2|30.98|42.57|21.62|
|NanoPi M4|![](/images/nanopim4.jpg)|RK3399<br /><br />A72 1.8GHz x 2<br />A53 1.5GHz x 4|43.73|64.28|27.43|
|Raspberry Pi 4B|![](/images/rasp4b.jpg)|BCM2711B0<br /><br />A72 1.5GHz x 4|58.38|71.59|37.93|
|EAIDK 310|![](/images/eaidk310.jpg)|RK3228H<br /><br />A53 1.3GHz x 4|68.97|90.87|48.22|
|Raspberry Pi 3B+|![](/images/rasp3b.jpg)|BCM2837B0<br /><br />A53 1.4GHz x 4|93.48|111.72|63.71|
|Raspberry Pi Zero 2W|![](/images/raspz2.jpg)|BCM2710A1<br /><br />A53 1.0GHz x 4|119.52|162.60|72.72|
|Loongson Pie Lite|![](/images/ls2k.jpg)|Loongson 2K1000<br /><br />GS264 1.0GHz x 2|185.28|276.03|124.39|
|Banana Pi M2 Zero 2|![](/images/bananaz2.jpg)|AllWinner H2+<br /><br />A7 1.2GHz x 4|230.97|327.65|147.97|
|PICO-PI-IMX7|![](/images/pico.jpg)|i.MX7D<br /><br />A7 1.0GHz x 2|220.10|366.92|137.02|
|NeZha D1|![](/images/nezhad1.jpg)|D1 C906<br /><br />RV64GCV 1GHz x 1|408.03|731.92|466.21|
