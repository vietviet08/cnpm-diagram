@startuml
actor "Job Seeker" as JS
actor "Employer" as E
participant "Job Portal System" as JPS
participant "Authentication Service" as AS

JS -> JPS: Đăng nhập
E -> JPS: Đăng nhập
JPS -> AS: Xác thực thông tin đăng nhập
AS -> JPS: Yêu cầu xác thực 2 bước
JPS -> JS: Xác thực 2 bước
JPS -> E: Xác thực 2 bước
JS -> JPS: Nhập mã xác thực
E -> JPS: Nhập mã xác thực
JPS -> AS: Xác thực mã
AS -> JPS: Xác thực thành công
JPS -> JS: Đăng nhập thành công
JPS -> E: Đăng nhập thành công
JPS -> JS: Khôi phục mật khẩu (nếu cần)
JPS -> E: Khôi phục mật khẩu (nếu cần)

@enduml