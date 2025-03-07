@startuml
left to right direction

skinparam actor {
  BackgroundColor LightGreen
  BorderColor Green
  FontColor DarkGreen
}

actor "Employer" as E

rectangle "Chức năng nhà tuyển dụng" {
  E --> (Đăng ký tài khoản)
  (Đăng ký tài khoản) <.. (Xác thực email) : <<include>>
  (Đăng ký tài khoản) <.. (Nhập thông tin công ty) : <<include>>

  E --> (Đăng nhập)
  (Đăng nhập) <.. (Xác thực 2 bước) : <<include>>

  E --> (Đăng tin tuyển dụng)
  (Đăng tin tuyển dụng) <.. (Nhập mô tả công việc) : <<include>>
  (Đăng tin tuyển dụng) <.. (Nhập yêu cầu công việc) : <<include>>
  (Đăng tin tuyển dụng) .> (Kiểm duyệt tin) : <<extends>>
  (Kiểm duyệt tin) <.. (Xác thực thông tin công ty) : <<include>>
}
@enduml