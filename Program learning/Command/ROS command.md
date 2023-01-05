---
tags: programming, command
---
# Error : dpkg...
[Tutorial 1]([https://brandviser.com.au/how-to-fix-dpkg-was-interrupted-error-linux/)
[Tutorial 2](https://blog.csdn.net/sinat_39150454/article/details/73466542)

# Error : roscore
## bashrc出問題 
看最後幾行 路徑source之類的有沒有設定好
> gedit ~/.bashrc

## 背景有其他core或master在跑
To kill roscore
> killall -9 roscore
> killall -9 rosmaster


# ROStopic
> rostopic list
> rostopic info
> rostopic echo

# Before excuting
>catkin_make
>catkin_make_isolated 
>source devel/setup.bash