@startuml
scale 350 width

[*] --> XemDanhSách : Bắt đầu quản lý tin tuyển dụng

state XemDanhSách {
  [*] --> XemDanhSáchTin
  XemDanhSáchTin : Nhà tuyển dụng xem danh sách tin tuyển dụng
  XemDanhSáchTin --> CậpNhậtTin : Cập nhật tin tuyển dụng
  CậpNhậtTin : [*] --> XóaTin : Tin tuyển dụng bị xóa
  XóaTin : [*] --> [*] : Quản lý tin tuyển dụng hoàn tất
}

@enduml