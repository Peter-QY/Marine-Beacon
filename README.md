# Marine-Beacon
## 海上信标

简介：这是2025年海洋航行器设计大赛 走向深蓝队的项目，赛道为新概念A1。

*本工程基于STM32F10ZET6搭建*

## 所使用的配件

正点原子STM32F103ZET6最小系统板

5v 8v稳压扩展版

DS18B20放水型温度传感器

水深传感器

24位高精度ADC转化模块

GPS模块

Lora模块*2

太阳能板

远程烧录模块*2

防水密封舱、防水螺栓

热熔胶、防水胶、电工胶布若干

1块3s航模电池

3个25kg防水舵机

1个25kg防水舵机

接线若干

碳板、打印件若干

## IO口功能分配

### 串口区

- 串口1 OPEMNMV
 
  USART1_TX  PA9
  
  USART1_RX  PA10
  
- 串口2 Lora模块
  
  USART2_TX  PD5      重定义而来

  USART2_RX  PD6      重定义而来
  
- 串口3 GPS定位模块 
  
  USART3_TX  PB10     
  
  USART3_RX  PB11      
- 串口4 （空闲）
  
  UART4_TX  PC10
  
  UART4_RX  PC11
  
- 串口5 （空闲） 
  
  UART5_TX   PC12
  
  UART5_RX   PD2


### I2C

  SCL    PD4
  
  SDA    PD1

### 舵机区

- Servo1   注射器1推动
  
  TIM3_CH1 PA6        输出PWM波
  
- Servo2  注射器2推动
  
  TIM3_CH2 PA7        输出PWM波
  
- Servo3  注射器3推动
  
  TIM3_CH3 PB0        输出PWM波

- Servo4  OPENMV云台转动
  
  TIM3_CH4 PB1        输出PWM波

