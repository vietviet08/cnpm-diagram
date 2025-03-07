@startuml
scale 350 width

[*] --> CậpNhậtThôngTin : Bắt đầu quản lý hồ sơ cá nhân

state CậpNhậtThôngTin {
  [*] --> NhậpThôngTinCáNhân
  NhậpThôngTinCáNhân : Ứng viên nhập thông tin cá nhân
  NhậpThôngTinCáNhân --> GửiThôngTin : Nhập xong thông tin
  GửiThôngTin : [*] --> CậpNhậtCV : Gửi thông tin
}

state CậpNhậtCV {
  [*] --> NhậpCV
  NhậpCV : Ứng viên nhập CV
  NhậpCV --> GửiCV : Nhập xong CV
  GửiCV : [*] --> CậpNhậtKỹNăng : Gửi CV
}

state CậpNhậtKỹNăng {
  [*] --> NhậpKỹNăng
  NhậpKỹNăng : Ứng viên nhập kỹ năng
  NhậpKỹNăng --> GửiKỹNăng : Nhập xong kỹ năng
  GửiKỹNăng : [*] --> TốiƯuHồSơ : Gửi kỹ năng
}

state TốiƯuHồSơ {
  [*] --> PhânTíchHồSơ
  PhânTíchHồSơ : Phân tích hồ sơ bằng AI
  PhânTíchHồSơ --> HồSơTốiƯu : Hồ sơ tối ưu
}

TốiƯuHồSơ --> [*] : Tối ưu hồ sơ hoàn tất

@enduml