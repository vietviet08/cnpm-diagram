@startuml
left to right direction

actor "Admin" as A

rectangle "Chức năng quản lý công việc" {
  A --> (Quản lý công việc)
  (Quản lý công việc) <.. (Xem danh sách công việc) : <<include>>
  (Quản lý công việc) .> (Gỡ bỏ công việc vi phạm) : <<extends>>
  (Gỡ bỏ công việc vi phạm) <.. (Xác minh vi phạm) : <<include>>
}

@enduml