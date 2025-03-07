@startuml
scale 350 width

[*] --> XemDanhSách : Bắt đầu quản lý lịch phỏng vấn

state XemDanhSách {
  [*] --> XemDanhSáchLịch
  XemDanhSáchLịch : Nhà tuyển dụng xem danh sách lịch phỏng vấn
  XemDanhSáchLịch --> CậpNhậtLịch : Cập nhật lịch phỏng vấn
  CậpNhậtLịch : [*] --> HủyLịch : Cập nhật lịch phỏng vấn
  HủyLịch : [*] --> [*] : Quản lý lịch phỏng vấn hoàn tất
}

@enduml