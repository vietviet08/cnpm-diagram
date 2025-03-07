@startuml
left to right direction

actor "Employer" as E

rectangle "Chức năng đăng tin tuyển dụng" {
  E --> (Đăng tin tuyển dụng)
  (Đăng tin tuyển dụng) <.. (Nhập mô tả công việc) : <<include>>
  (Đăng tin tuyển dụng) <.. (Nhập yêu cầu công việc) : <<include>>
  (Đăng tin tuyển dụng) .> (Kiểm duyệt tin) : <<extends>>
  (Kiểm duyệt tin) <.. (Xác thực thông tin công ty) : <<include>>
}

@enduml