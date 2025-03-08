@startuml
left to right direction

actor "Job Seeker" as JS
actor "Employer" as E

rectangle "Chức năng đăng nhập" {
  JS --> (Đăng nhập)
  E --> (Đăng nhập)
  (Đăng nhập) <.. (Xác thực 2 bước) : <<include>>
  (Đăng nhập) .> (Khôi phục mật khẩu) : <<extends>>
}

@enduml