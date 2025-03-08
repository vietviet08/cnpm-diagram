@startuml
scale 350 width

[*] --> NhậpThôngTinĐăngNhập : Bắt đầu đăng nhập

state NhậpThôngTinĐăngNhập {
  [*] --> NhậpThôngTin
  NhậpThôngTin : Người dùng nhập thông tin đăng nhập
  NhậpThôngTin --> GửiThôngTin : Nhập xong thông tin
  GửiThôngTin : [*] --> XácThựcHaiLớp : Gửi thông tin đăng nhập
}

state XácThựcHaiLớp {
  [*] --> GửiMãXácThực : Gửi mã xác thực
  GửiMãXácThực --> ChờXácThực : Mã xác thực đã gửi
  ChờXácThực --> XácThựcThànhCông : [*] : Mã xác thực đúng
  ChờXácThực --> XácThựcThấtBại : [*] : Mã xác thực sai
  XácThựcThấtBại --> KhôiPhụcMậtKhẩu : Người dùng chọn khôi phục mật khẩu
  KhôiPhụcMậtKhẩu --> NhậpThôngTinĐăngNhập : Mật khẩu được khôi phục
}

XácThựcHaiLớp --> ĐăngNhậpThànhCông : [*] : Xác thực thành công
ĐăngNhậpThànhCông --> [*] : Đăng nhập hoàn tất

@enduml