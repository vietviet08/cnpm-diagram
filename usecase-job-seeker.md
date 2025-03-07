@startuml
left to right direction

skinparam actor {
  BackgroundColor LightGreen
  BorderColor Green
  FontColor DarkGreen
}

actor "Job Seeker" as JS
actor "AI Chatbot" as AI

rectangle "Chức năng ứng viên" {
  JS --> (Đăng ký tài khoản)
  (Đăng ký tài khoản) <.. (Xác thực email) : <<include>>
  (Đăng ký tài khoản) <.. (Nhập thông tin cá nhân) : <<include>>
  (Đăng ký tài khoản) .> (Gợi ý tối ưu hồ sơ bằng AI) : <<extends>>

  JS --> (Đăng nhập)
  (Đăng nhập) <.. (Xác thực 2 bước) : <<include>>
  (Đăng nhập) .> (Khôi phục mật khẩu) : <<extends>>

  JS --> (Tìm kiếm công việc)
  (Tìm kiếm công việc) <.. (Lọc theo ngành nghề) : <<include>>
  (Tìm kiếm công việc) <.. (Lọc theo địa điểm) : <<include>>
  (Tìm kiếm công việc) <.. (Lọc theo mức lương) : <<include>>
  (Tìm kiếm công việc) .> (Gợi ý việc làm phù hợp) : <<extends>>
  (Gợi ý việc làm phù hợp) <.. (Phân tích hồ sơ bằng AI) : <<include>>
}
@enduml