* Để có thể xem lịch sử hiển thị/ cuộn trang trong tmux, ta phải đi vào copy mode:
   ```<Prefix> - [```

* Thóat khỏi Copy mode:
   ```q```

* Di chuyển trong copy mode:
   + Bằng vim key:
      - lên xuống qua lại: h/j/k/l
      - trang trước trang sau: Ctrl - b, Ctrl - f
      - đầu trang, cuối trang: gg, gG

   + Hoặc là các phím mũi tên và PageUp, PageDown, Home, End

* Sao chép chuỗi ký tự trên màn hình: (lưu ý là ta phải vào copy mode rồi)
   + bắt đầu sao chép từ vị trí con trỏ:
      v
   + dùng các phím di chuyển để chọn chuỗi
   + kết thúc quá trình chọn (và tự động thóat khỏi copy mode)
      y
   + truy cập đến nơi cần dán chuỗi (VIM hoặc là dấu nhắc command line)
   + dán chuỗi
      ```<Prefix> - ]```

* Mặc định của bộ nhớ lịch sử hiển thị trong tmux chỉ khỏang 1000 dòng cho 1 "Pane"
  Để có thể lưu giữ được nhiều lịch sử hiển thị hơn ta có thể thêm dòng sau vào file .tmux.conf

   set-option -g history-limit 5000
