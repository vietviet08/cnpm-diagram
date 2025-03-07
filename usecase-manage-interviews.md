@startuml
left to right direction

actor "Employer" as E

rectangle "Chức năng quản lý lịch phỏng vấn" {
  E --> (Quản lý lịch phỏng vấn)
  (Quản lý lịch phỏng vấn) <.. (Xem danh sách lịch phỏng vấn) : <<include>>
  (Quản lý lịch phỏng vấn) <.. (Cập nhật lịch phỏng vấn) : <<include>>
  (Quản lý lịch phỏng vấn) <.. (Hủy lịch phỏng vấn) : <<include>>
}

@enduml