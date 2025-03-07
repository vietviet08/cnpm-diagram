@startuml
scale 350 width

[*] --> XemDanhSách : Bắt đầu quản lý công việc

state XemDanhSách {
  [*] --> XemDanhSáchCôngViệc
  XemDanhSáchCôngViệc : Quản trị viên xem danh sách công việc
  XemDanhSáchCôngViệc --> ChọnCôngViệc : Chọn công việc vi phạm
  ChọnCôngViệc : [*] --> GỡBỏViPham : Chọn công việc vi phạm
}

state GỡBỏViPham {
  [*] --> XácMinhViPham : Xác minh vi phạm
  XácMinhViPham --> [*] : Công việc bị gỡ bỏ
}

@enduml