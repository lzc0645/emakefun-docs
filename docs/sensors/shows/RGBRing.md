# 12位RGB灯环模块规格书

## 模块图

![01](12位RGB灯环图片/01.jpg)

## 概述

​        WS2812是一个集控制电路与发光电路于一体的智能外控LED光源。其外型与一个5050LED灯珠相同， 每个元件即为一个像素点。像素点内部包含了智能数字接口数据锁存信号整形放大驱动电路， 还包含有高精度的内部振荡器和12V高压可编程定电流控制部分，有效保证了像素点光的颜色高度一致。数据协议采用单线归零码的通讯方式，像素点在上电复位以后，DIN端接受从控制器传输过来的数据，首先送过来的24bit数据被第一个像素点提取后，送到像素点内部的数据锁存器，剩余的数据经过内部整形处理电路整形放大后通过DO端口开始转发输出给下一个级联的像素点，每经过一个像素点的传输，信号减少24bit。像素点采用自动整形转发技术，使得该像素点的级联个数不受信号传送的限制，仅仅受限信号传输速度要求。LED具有低电压驱动，环保节能，亮度高，散射角度大，一致性好，超低功率，超长寿命等优点。将控制电路集成于上面，电路变得更加简单，体积小，安装更加简便。

## 原理图

![1](12位RGB灯环图片/1.png)

## 模块参数

| 引脚名称 | 描述         |
| -------- | ------------ |
| V        | 5V电源引脚   |
| G        | GND 地线     |
| DI       | 信号输入引脚 |
| DO       | 信号输出引脚 |

## 详细原理图

 [RGB-ring.pdf](12位RGB灯环图片/RGB-ring.pdf) 

## 机械尺寸

![6](12位RGB灯环图片/6.png)