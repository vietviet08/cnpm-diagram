@startuml
left to right direction

actor "Employer" as E
actor "Job Seeker" as JS

rectangle "Chức năng tạo lịch phỏng vấn" {
  E --> (Tạo lịch phỏng vấn)
  (Tạo lịch phỏng vấn) <.. (Chọn thời gian phỏng vấn) : <<include>>
  (Tạo lịch phỏng vấn) <.. (Chọn địa điểm phỏng vấn) : <<include>>
  (Tạo lịch phỏng vấn) <.. (Gửi thông báo phỏng vấn) : <<include>>
  JS <.. (Nhận thông báo phỏng vấn) : <<include>>
}

@enduml