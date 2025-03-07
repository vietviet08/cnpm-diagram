@startuml
scale 350 width

[*] --> ChọnCôngViệc : Bắt đầu nộp đơn xin việc

state ChọnCôngViệc {
  [*] --> ChọnCôngViệcCụThể
  ChọnCôngViệcCụThể : Ứng viên chọn công việc
  ChọnCôngViệcCụThể --> GửiCôngViệc : Gửi công việc
  GửiCôngViệc : [*] --> ĐínhKèmCV : Gửi công việc
}

state ĐínhKèmCV {
  [*] --> ĐínhKèmThư : Đính kèm CV
  ĐínhKèmThư --> PhânTíchCV : Đính kèm thư xin việc
  PhânTíchCV : [*] --> HoànTấtNộpĐơn : Phân tích CV bằng AI
}

ĐínhKèmCV --> PhânTíchCV : Đính kèm xong
PhânTíchCV --> HoànTấtNộpĐơn : Phân tích xong
HoànTấtNộpĐơn --> [*] : Nộp đơn hoàn tất

@enduml