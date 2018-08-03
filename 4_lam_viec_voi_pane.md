* Tạo Pane mới:
   + Chia đôi 1 pane thành 2 pane theo chiều dọc:
      ```<Prefix> -  v```
   + Chia đôi 1 pane thành 2 pane theo chiều ngang:
      ```<Prefix> -  s```
* Xóa một Pane:
   ```<Prefix> - C```

* Di chuyển giữa các pane:
   + cách 1: di chuyển bằng cách nhấn số thứ tự của pane đó
      ```<Prefix> - q - <số thứ tự của pane muốn tới:0, 1, 2...>```

   + cách 2: di chuyển theo phong cách của VIM
      - qua Pane bên trái:
         ```Alt - h```
      - qua Pane bên phải:
         ```Alt - l```
      - lên Pane phía trên:
         ```Alt - k```
      - xuống Pane phía dưới:
         ```Alt - j```
      - Chuyển tới pane trước đó mới truy cập tới:
         ```<Prefix> - Tab```
     
* Mở rộng một Pane tòan màng hình/ trở về trạng thái ban đầu (toggle fullscreen)
   ```<Prefix> - z ```

* Thay đổi kích thước của một pane: mở rộng/thu hẹp lên/xuống trái/phải
	+ Dùng hotkey:
	   ```<Prefix> - <Up Arrow>```
	   ```<Prefix> - <Down Arrow>```
	   ```<Prefix> - <Left Arrow>```
	   ```<Prefix> - <Right Arrow>```

	+ Dùng lệnh: resize-pane (tham khảo cách gõ lệnh cho tmux trong phấn 1_cai_dat_va_bat_dau_su_dung.txt) 
		VD: để thay đổi chiều cao của một pane thành 8 dòng.
			 :resize-pane -y8

* Thay đổi vị trí của pane trong 1 window: 
	+ chuyển pane hiện tại đến vị trí trước đó:
		```<Prefix> - {```
	+ chuyển pane hiện tại đến vị trí tiếp theo:
		```<Prefix> - }```

* Di chuyển pane giữa các window:
	+ chuyển pane hiện tại ra một window mới:
		```<Prefix> - !```
	+ chuyển pane hiện tại đến window đã được tạo rồi:
		VD: chuyển pane hiện tại tới window 2
		:join-pane -t 2
		VD: chuyển window 2 thành một pane trong window hiện tại
		:join-pane -s 2

* Thay đổi layout của các panes: (từ chia ngang sang chia dọc)
		```<Prefix> - "khoảng trắng"```

* Phần tiếp theo [Copy mode trong tmux](https://github.com/kuonvu/su_dung_tmux/blob/master/5_copy_mode_trong_tmux.md)