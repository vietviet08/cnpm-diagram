@startuml
scale 350 width

[*] --> NhậpThôngTin : Bắt đầu đăng ký

state NhậpThôngTin {
  [*] --> NhậpThôngTinCáNhân
  NhậpThôngTinCáNhân : Người dùng nhập thông tin cá nhân
  NhậpThôngTinCáNhân --> GửiThôngTin : Nhập xong thông tin
  GửiThôngTin : [*] --> XácThựcEmail : Gửi thông tin
}

state XácThựcEmail {
  [*] --> GửiEmailXácThực : Gửi email xác thực
  GửiEmailXácThực --> ChờXácThực : Email đã gửi
  ChờXácThực --> XácThựcThànhCông : [*] : Email xác thực thành công
  ChờXácThực --> XácThựcThấtBại : [*] : Email xác thực thất bại
  XácThựcThấtBại --> NhậpThôngTin : Người dùng nhập lại thông tin
}

XácThựcEmail --> TốiƯuHồSơ : [*] : Email xác thực thành công

state TốiƯuHồSơ {
  [*] --> PhânTíchHồSơ : Phân tích hồ sơ bằng AI
  PhânTíchHồSơ --> HồSơTốiƯu : Hồ sơ tối ưu
}

TốiƯuHồSơ --> ĐăngKýThànhCông : Hồ sơ tối ưu thành công
ĐăngKýThànhCông --> [*] : Đăng ký hoàn tất

@enduml