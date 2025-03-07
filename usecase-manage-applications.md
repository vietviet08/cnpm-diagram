@startuml
left to right direction

actor "Job Seeker" as JS

rectangle "Chức năng quản lý đơn xin việc" {
  JS --> (Quản lý đơn xin việc)
  (Quản lý đơn xin việc) <.. (Xem trạng thái đơn) : <<include>>
  (Quản lý đơn xin việc) <.. (Hủy đơn xin việc) : <<include>>
  (Quản lý đơn xin việc) <.. (Cập nhật đơn xin việc) : <<include>>
}

@enduml