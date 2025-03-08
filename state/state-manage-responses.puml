@startuml
scale 350 width

[*] --> XemDanhSách : Bắt đầu quản lý phản hồi ứng viên

state XemDanhSách {
  [*] --> XemDanhSáchỨngViên
  XemDanhSáchỨngViên : Nhà tuyển dụng xem danh sách ứng viên
  XemDanhSáchỨngViên --> PhảnHồi : Phản hồi ứng viên
  PhảnHồi : [*] --> LênLịchPhỏngVấn : Lên lịch phỏng vấn
  LênLịchPhỏngVấn : [*] --> [*] : Quản lý phản hồi hoàn tất
}

@enduml