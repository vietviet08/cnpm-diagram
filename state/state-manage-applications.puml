@startuml
scale 350 width

[*] --> XemTrạngThái : Bắt đầu quản lý đơn xin việc

state XemTrạngThái {
  [*] --> XemTrạngTháiĐơn
  XemTrạngTháiĐơn : Ứng viên xem trạng thái đơn
  XemTrạngTháiĐơn --> HủyĐơn : Hủy đơn xin việc
  HủyĐơn : [*] --> ĐơnHủy : Đơn xin việc bị hủy
  ĐơnHủy --> CậpNhậtĐơn : Cập nhật đơn xin việc
  CậpNhậtĐơn : [*] --> [*] : Cập nhật đơn hoàn tất
}

@enduml