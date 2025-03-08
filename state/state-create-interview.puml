@startuml
scale 350 width

[*] --> ChọnThờiGian : Bắt đầu tạo lịch phỏng vấn

state ChọnThờiGian {
  [*] --> ChọnThờiGianCụThể
  ChọnThờiGianCụThể : Nhà tuyển dụng chọn thời gian phỏng vấn
  ChọnThờiGianCụThể --> GửiThờiGian : Gửi thời gian
  GửiThờiGian : [*] --> ChọnĐịaĐiểm : Gửi thời gian
}

state ChọnĐịaĐiểm {
  [*] --> ChọnĐịaĐiểmCụThể
  ChọnĐịaĐiểmCụThể : Nhà tuyển dụng chọn địa điểm phỏng vấn
  ChọnĐịaĐiểmCụThể --> GửiĐịaĐiểm : Gửi địa điểm
  GửiĐịaĐiểm : [*] --> GửiThôngBáo : Gửi địa điểm
}

state GửiThôngBáo {
  [*] --> GửiEmail
  GửiEmail : Gửi thông báo phỏng vấn
  GửiEmail : [*] --> [*] : Gửi thông báo hoàn tất
}

@enduml