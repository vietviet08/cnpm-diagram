@startuml
scale 350 width

[*] --> XemDanhSách : Bắt đầu quản lý người dùng

state XemDanhSách {
  [*] --> XemDanhSáchNgườiDùng
  XemDanhSáchNgườiDùng : Quản trị viên xem danh sách người dùng
  XemDanhSáchNgườiDùng --> ChọnNgườiDùng : Chọn người dùng để cập nhật thông tin
  ChọnNgườiDùng : [*] --> CậpNhậtThôngTin : Chọn người dùng
}

state CậpNhậtThôngTin {
  [*] --> GửiThôngTin : Gửi thông tin cập nhật
  GửiThôngTin --> KhóaTàiKhoản : Khóa tài khoản vi phạm
}

CậpNhậtThôngTin --> KhóaTàiKhoản : Gửi thông tin cập nhật

state KhóaTàiKhoản {
  [*] --> XácMinhViPham : Xác minh vi phạm
  XácMinhViPham --> [*] : Hoàn tất quản lý người dùng
}

@enduml