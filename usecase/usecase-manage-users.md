@startuml
left to right direction

actor "Admin" as A

rectangle "Chức năng quản lý người dùng" {
  A --> (Quản lý người dùng)
  (Quản lý người dùng) <.. (Xem danh sách người dùng) : <<include>>
  (Quản lý người dùng) <.. (Cập nhật thông tin người dùng) : <<include>>
  (Quản lý người dùng) .> (Khóa tài khoản vi phạm) : <<extends>>
  (Khóa tài khoản vi phạm) <.. (Xác minh vi phạm) : <<include>>
}

@enduml