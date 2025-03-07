@startuml
left to right direction

actor "Job Seeker" as JS

rectangle "Chức năng nộp đơn xin việc" {
  JS --> (Nộp đơn xin việc)
  (Nộp đơn xin việc) <.. (Chọn công việc) : <<include>>
  (Nộp đơn xin việc) <.. (Đính kèm CV) : <<include>>
  (Nộp đơn xin việc) <.. (Đính kèm thư xin việc) : <<include>>
  (Nộp đơn xin việc) .> (Phân tích CV bằng AI) : <<extends>>
}

@enduml