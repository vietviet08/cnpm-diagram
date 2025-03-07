@startuml
left to right direction

actor "Job Seeker" as JS

rectangle "Chức năng đăng ký tài khoản" {
  JS --> (Đăng ký tài khoản)
  (Đăng ký tài khoản) <.. (Xác thực email) : <<include>>
  (Đăng ký tài khoản) <.. (Nhập thông tin cá nhân) : <<include>>
  (Đăng ký tài khoản) .> (Gợi ý tối ưu hồ sơ bằng AI) : <<extends>>
}

@enduml