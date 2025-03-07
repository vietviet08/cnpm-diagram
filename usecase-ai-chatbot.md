@startuml
left to right direction

actor "Job Seeker" as JS

rectangle "Chức năng AI Chatbot" {
  JS --> (Chatbot AI hỗ trợ tìm việc)
  (Chatbot AI hỗ trợ tìm việc) .> (Gợi ý việc làm phù hợp) : <<extends>>
  (Chatbot AI hỗ trợ tìm việc) .> (Tư vấn phỏng vấn) : <<extends>>
  (Tư vấn phỏng vấn) <.. (Gợi ý câu hỏi phỏng vấn) : <<include>>
  (Gợi ý việc làm phù hợp) <.. (Đánh giá CV bằng AI) : <<include>>
}

@enduml