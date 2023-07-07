# USBTO3DO-SANYO-IMP21J
这是Francois CARON的SATATO3DO项目https://github.com/FCare/SataTo3DO 的拓展，使用了集成电路来缩小体积，具体使用方法请参考其方案。（注意此站点源代码已更新，不要直接使用已编译好的UF2文件，需要重新编译UF2文件后使用）





关于UF2文件，注意此站点源代码已更新，不要直接使用已编译好的UF2文件。
如何获得一个可以使用的UF2文件：
方法1.请自行重新编译源文件文件获得一个新UF2文件；
方法2.经Francois CARON授权，如果你只是为自己制作，非用于商业用途，可以联系我推特@TZMWXdiyer获得新UF2文件。请不要再发邮件打扰Francois CARON先生。





BOM: 最小系统：

U1 RP2040 PICO模块(兼容引脚功能看2040pico.jpg）

U2/U3 TXS0108 TSSOP-20

U4 74LVC4245 TSSOP-24

X1 有源晶振OSC SMD7050 16.93Mhz

POWER FFC插座14P 1.25mm  （FFC & FPC Connectors POST PLATED VERT 14P 1.25mm）

CDROM FFC插座30P 1.25mm  （FFC & FPC Connectors POST PLATED VERT 30P 1.25mm）

注意：注意：注意：需要去除主板上的电池旁边的C53电容

如果你要在模块上建立一个读盘灯（同主机面板绿色读盘灯）：

你需要增加： R1：470Ω（SMD0603 或直插） LED：3MM（直插）

预留了电容的位置，可以不需要安装， C1/C2：220uf-470uf/10V(直插） C3/C4/C5/C6：0.1uf（SMD0603）

反面预留了(+5V,D-,D+,GND)接口，可以安装一个USB母座，注意此接口要与2040模块要焊接连线，具体方法请参考PCB背面图示:注意，这里并没有HUB功能，只能使用其中的一个，其意义是省去一根TYPE-C的转换线。

注意：此板可零时用于GOLDSTAR_GDO101M的使用，请勿长期使用
