# 硬體 
1. Pixhawk
	- 飛控板
	- 32bit
2. APM 
	- 飛控板
	- 8 bit
	- 基於arduino

# 軟體
1. PX4
2. ArduPilot

# PPM 訊號
1. 把多路通道(遙控器)的pwm訊號調製到一路通道上, 傳輸到接收機後, 再由接收機還原成多路PWM從各個通道輸出
2. Pixhawk只接收PPM訊號

# 