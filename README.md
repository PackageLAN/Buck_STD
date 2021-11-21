# Buck_STD
## 这是一个学习项目，一个缝合出来的，尽量使用分立器件的Buck DC-DC。
一些参考文章或博客内容链接如下：  
  
电感的电流方向检测：[P-MOSFET做理想二极管](https://www.brobwind.com/archives/1204)  
用了电流镜的原理，为了有足够时间关断下侧N-MOSFET，设置电流镜的下拉电阻为不对称的，于是对于比较器的差模输入来说过零点提前了，设计中使用了分压是为了保证输入的共模电压不超出比较器的电压轨。  

---
DC-DC的环路补偿-电压模式（Page8）：[开关模式电源的建模和环路补偿设计](https://www.analog.com/media/cn/technical-documentation/application-notes/AN149f_chs.pdf)  
我控制理论学得不行，所以参数是随便调的，为了方便只用了Ⅱ型环路补偿。  

---
功率N-MOSFET半桥的驱动：(没有链接)  
双十一捡的电子垃圾（一个未知型号的BLDC驱动板）上抄过来的，具有可调整的死区以及MOSFET开通的斜率控制（通过改变电阻阻值）。
