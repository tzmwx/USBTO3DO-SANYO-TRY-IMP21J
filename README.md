# USBTO3DO-SANYO-IMP21J
这是Francois CARON的SATATO3DO项目https://github.com/FCare/SataTo3DO 的拓展，使用了集成电路来缩小体积，具体使用方法请参考其方案

BOM: 最小系统：

U1 RP2040 PICO模块(兼容引脚功能看2040pico.jpg）

U2/U3 TXS0108 TSSOP-20

U4 74LVC4245 TSSOP-24

X1 有源晶振OSC SMD7050 16.93Mhz

需要去除主板上的电池旁边的C53电容

如果你要在模块上建立一个读盘灯（同主机面板绿色读盘灯）：

你需要增加： R1：470欧姆 LED：3MM

预留了电容的位置，可以不需要安装， C1/C2：220uf-470uf/10V C3/C4/C5/C6：0.1uf

反面预留了(+5V,D-,D+,GND)接口，可以安装一个USB母座，注意此接口要与2040模块要焊接连线
