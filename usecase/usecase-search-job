@startuml
left to right direction

actor "Job Seeker" as JS
actor "AI Chatbot" as AI

rectangle "Chức năng tìm kiếm công việc" {
  JS --> (Tìm kiếm công việc)
  (Tìm kiếm công việc) <.. (Lọc theo ngành nghề) : <<include>>
  (Tìm kiếm công việc) <.. (Lọc theo địa điểm) : <<include>>
  (Tìm kiếm công việc) <.. (Lọc theo mức lương) : <<include>>
  (Tìm kiếm công việc) .> (Gợi ý việc làm phù hợp) : <<extends>>
  (Gợi ý việc làm phù hợp) <.. (Phân tích hồ sơ bằng AI) : <<include>>
  JS --> (Chatbot AI hỗ trợ tìm việc)
  (Chatbot AI hỗ trợ tìm việc) .> (Gợi ý việc làm phù hợp) : <<extends>>
}

@enduml