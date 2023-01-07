---
tags: programming, command
---
# Run application
> obsidian
> ./QGroundControl.AppImage


# Adjust the brightness of the second monitor
> sudo ddcutil --display 1 setvcp 10 0
	
	
# Tmux

- Ctrl+b 再輸入 % 垂直分割視窗。
- Ctrl+b 再輸入 " 水平分割視窗。
- Ctrl+b 再輸入 o 以輪流方式輪流切換 pane。
- Ctrl+b 再輸入 方向鍵 切換至指定方向的 pane。
- Ctrl+b 再輸入 空白鍵 切換佈局。
- Ctrl+b 再輸入 ! 將目前的 pane 抽出來，獨立建立一個 window 視窗。
- Ctrl+b 再輸入 x 關閉目前的 pane。
# Clean up redundant packages
> sudo apt autoremove
> sudo apt autoclean

# Copy to dir
> cp *file name* *dir*

# Memory
- Clean up packages
	> sudo apt autoremove
	> sudo apt autoclean
- RAM in real time
	> watch -n 1 free -m
- Release cached pages, inodes, and directory entries
	> sudo sync
	> sudo sysctl -w vm.drop_caches=3
- Remove the old logs
	> sudo journalctl --vacuum-``time``=2d;

# Generic
- 查看有安裝的版本
	> dpkg --get-selections | grep linux-image

- 移除deinstall
	> sudo dpkg -P linux-image-x.xxx.xx-generic

# Cool effects
> cmatrix
> hollywood (電腦會燒)

