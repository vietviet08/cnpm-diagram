@startuml
left to right direction

actor "Employer" as E

rectangle "Chức năng quản lý tin tuyển dụng" {
  E --> (Quản lý tin tuyển dụng)
  (Quản lý tin tuyển dụng) <.. (Xem danh sách tin tuyển dụng) : <<include>>
  (Quản lý tin tuyển dụng) <.. (Cập nhật tin tuyển dụng) : <<include>>
  (Quản lý tin tuyển dụng) <.. (Xóa tin tuyển dụng) : <<include>>
}

@enduml