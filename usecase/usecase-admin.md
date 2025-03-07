@startuml
left to right direction

skinparam actor {
  BackgroundColor LightGreen
  BorderColor Green
  FontColor DarkGreen
}

actor "Admin" as A

rectangle "Chức năng quản trị viên" {
  A --> (Quản lý người dùng)
  (Quản lý người dùng) <.. (Xem danh sách người dùng) : <<include>>
  (Quản lý người dùng) <.. (Cập nhật thông tin người dùng) : <<include>>
  (Quản lý người dùng) .> (Khóa tài khoản vi phạm) : <<extends>>
  (Khóa tài khoản vi phạm) <.. (Xác minh vi phạm) : <<include>>

  A --> (Quản lý công việc)
  (Quản lý công việc) <.. (Xem danh sách công việc) : <<include>>
  (Quản lý công việc) .> (Gỡ bỏ công việc vi phạm) : <<extends>>
  (Gỡ bỏ công việc vi phạm) <.. (Xác minh vi phạm) : <<include>>
}
@enduml