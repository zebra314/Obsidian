---
tags: programming, command
---
# Run application
> obsidian
> ./QGroundControl.AppImage
> sudo ./cleanup.sh

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

# Taskline (to manage tasks in terminal)
1.  board view
	> tl
2.  timeline view
	> tl -i
3.  create task
	> tl t
4.  create note
	> tl n
5.  create board
	> -b *board names*
	> Ex. tl t "Update contributing guidelines" -b coding,docs
6.  list items
	> tl l *board name*
7.  set duedate
	> tl t "*task name*" -b *board name* -d *dd.mm.yyyy HH:MM*
	> tl due *item ID* "*dd.mm.yyyy HH:MM"
	> *today* *tonight* *tomorrow* *next monday*
8.  set priority
	> -p *1 or 2 or 3*
	>  1 - Normal priority
	> 2- Medium priority
	> 3 - High priority
	> (before task created -p)
	> (after created p)
9. begin task
	> tl b *ID1*, *ID2*,.....
10.  check task
	> tl c *ID*
11. star
	> tl s *ID*
12.  find items
	> tl f *item name*
13. display archive
	> tl a
14.  cancel
	> tl cancel
15.  delete
	> tl d *ID*
16.  delete checked tasks
	> tl clear



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

