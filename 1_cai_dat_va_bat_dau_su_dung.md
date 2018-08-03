### Cài đặt chương trình:
   * ubuntu:
      ``` $ sudo apt-get install tmux ```
   * opensuse:
      ``` $ sudo zypper install tmux ```

* Chép file .tmux.conf mẫu trong reposity này vào thư mục "home" của mình:

* Lưu ý tổng quan về phím tắt trong tmux
   + Các phím tắt được giới thiệu trong hướng dẫn này có thể ko giống với bản TMUX nguyên gốc là
     do mình đã cấu hình lại TMUX bằng cách chỉnh sửa file [.tmux.conf](https://github.com/kuonvu/su_dung_tmux/blob/master/.tmux.conf)
     Do là người bị ảnh hưởng bởi VIM, nên thường các phím tắt được mình cấu hình khá giống với VIM.
   
     Tmux rất linh động trong việc cấu hình hotkey nên bạn có thể tùy ý thay đổi bằng việc chỉnh
     sửa file  [.tmux.conf](https://github.com/kuonvu/su_dung_tmux/blob/master/.tmux.conf) và sau đó tải lại câú hình này.

   + Khái niệm về "Prefix" hotkey:
     ```Prefix``` trong TMUX là bộ phím cần được nhấn trước khi nhấn một phím khác để hòan tất một chuỗi hotkey đầy đủ trong tmux.
     Trong truờng hợp của mình, mình dùng ```Ctrl-s```. Nguyên nhân là do ```Ctrl-s``` không trùng với hotkey trong linux command line interface.
     Mặc định của tmux là ```Ctrl-b```, nhưng hotkey này trùng với việc di chuyển con trỏ về phía bên trái trong linux comand line interface.

     Ví Dụ: Nếu thấy viết là ```<Prefix> - v```
         -> thì trong trường hợp ```Prefix``` là ```Ctrl-s``` -> mình phải nhấn 2 phím ```Ctrl```, ```s```, nhả 2 phím ra và sau đó là nhấn ```v  ```      

   + Hotkey của TMUX phân biệt chữ hoa chữ thường:
     Ví Dụ: Nếu thấy viết là ```<Prefix> - s```
         -> thì trong trường hợp ```Prefix``` là ```Ctrl-s``` -> mình phải nhấn 2 phím ```Ctrl```, ```s```, nhả 2 phím ra và sau đó là nhấn ```s```       
     Ví Dụ: Nếu thấy viết là ```<Prefix> - S```
         -> thì trong trường hợp ```Prefix``` là ```Ctrl-s``` -> mình phải nhấn 2 phím ```Ctrl```, ```s```, nhả 2 phím ra và sau đó là nhấn 2 phím ```Shift``` và ```s``` 

   + Một số Hotkey trong tmux có thể ko cần nhấn Prefix:
     Ví Dụ: Nếu thấy viết là ```Alt - s```
         -> thì chỉ cần nhấn 2 phím ```Alt``` và ```s``` cùng lúc

   + Cách để gõ lệnh cho tmux: 
    ```<Prefix>``` + ```":"```

    -> Gõ hotkey ```<Prefix>```, sau đó gõ dấu hai chấm

    Trong hướng dẫn này nếu thấy ghi ":xxxx" thì "xxxx chính là lệnh của tmux.

* Lưu ý về cấp bậc trong tmux:
   -> Một máy tính có thể có nhiều Tmux session chạy cùng lúc trên nó
      -> 1 session (một phiên làm việc) có thể chứa nhiều Window Tab
         -> 1 Window Tab có thể chứa nhiều Pane

Phần tiếp theo [Làm việc với session](https://github.com/kuonvu/su_dung_tmux/blob/master/2_lam_viec_voi_session.md)