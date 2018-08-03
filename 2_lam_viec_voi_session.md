* Tạo một session mới:
   ```$tmux new -s <tên_session>```

* Tạm ngưng một session: (nhưng session này vẫn tồn tại)
   ```<Prefix> - d```

* Chạy lại một session đã lưu:
   ```$tmux a -t <tên_session>```
	hoặc
	```$tmux attach -t <tên_session_hoặc_số_thứ_tự_session>```

* Liệt kê tất cả các session:
	```$tmux ls```

* Phần tiếp theo [Làm việc với windown tab](https://github.com/kuonvu/su_dung_tmux/blob/master/3_lam_viec_voi_window_tab.md)