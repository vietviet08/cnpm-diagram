@startuml
actor "Job Seeker" as JS
participant "Job Portal System" as JPS
participant "Email Service" as ES

JS -> JPS: Đăng ký tài khoản
JPS -> JPS: Nhập thông tin cá nhân
JPS -> ES: Gửi email xác thực
ES -> JS: Email xác thực
JS -> JPS: Xác thực email
JPS -> JPS: Gợi ý tối ưu hồ sơ bằng AI (nếu có)
JPS -> JS: Hoàn tất đăng ký

@enduml