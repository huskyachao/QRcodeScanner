# QRcodeScanner
The introduction of QRcode Scanner.

## Scanner结构及工作流程
  常见的平板式扫描枪一般由光源、光学透镜、扫描模组、模拟数字转换电路加塑料外壳构成。<br>
  它利用光电元件将检测到的光信号转换成电信号，再将电信号通过模拟数字转换器转化为数字信号传输到计算机中处理。当扫描一副图像的时候，光源照射到图像上后反射光穿过透镜会聚到扫描模组上，由扫描模组把光信号转换成模拟数字信号（即电压，它与接受到的光的强度有关），同时指出那个像数的灰暗程度。这时候模拟-数字转换电路把模拟电压转换成数字讯号，传送到电脑。颜色用RGB三色的8、10、12位来量化，既把信号处理成上述位数的图像输出。如果有更高的量化位数，意味着图像能有更丰富的层次和深度，但颜色范围已超出人眼的识别能力，所以在可分辨的范围内对于我们来说，更高位数的扫描枪扫描出来的效果就是颜色衔接平滑，能够看到更多的画面细节。
## 图像传感器 [Wiki](https://zh.wikipedia.org/wiki/%E5%9B%BE%E5%83%8F%E4%BC%A0%E6%84%9F%E5%99%A8)
### 1.CMOS [百度](https://baike.baidu.com/item/CMOS%E5%9B%BE%E5%83%8F%E4%BC%A0%E6%84%9F%E5%99%A8)
  CMOS图像传感器是一种典型的固体成像传感器，与CCD有着共同的历史渊源。CMOS图像传感器通常由像敏单元阵列、行驱动器、列驱动器、时序控制逻辑、`AD转换器`、数据总线输出接口、控制接口等几部分组成,这几部分通常都被集成在同一块硅片上。其工作过程一般可分为复位、光电转换、积分、读出几部分。<br>
  在CMOS图像传感器芯片上还可以集成其他数字信号处理电路，如`AD转换器`、自动曝光量控制、非均匀补偿、白平衡处理、黑电平控制、伽玛校正等，为了进行快速计算甚至可以将具有可编程功能的DSP器件与CMOS器件集成在一起，从而组成单片数字相机及图像处理系统。<br>
  噪声的大小直接影响CMOS图像传感器对信号的采集和处理，因此如何提高信噪比是CMOS图像传感器的关键技术之一。噪声主要包括散粒噪声、热噪声、1/f噪声、非均匀噪声和固定图像噪声。其中散粒噪声和热噪声是由载流子引起的，1/f噪声和非均匀噪声是由材料的缺陷和不均匀性引起的，固定图像噪声是因为工艺的误差使相邻输出信号的源跟随器不匹配引起的。
#### CMOS
### 2.CCD [百度](https://baike.baidu.com/item/CCD%E5%9B%BE%E5%83%8F%E4%BC%A0%E6%84%9F%E5%99%A8)
