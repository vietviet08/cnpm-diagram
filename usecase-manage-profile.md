@startuml
left to right direction

actor "Job Seeker" as JS

rectangle "Chức năng quản lý hồ sơ" {
  JS --> (Quản lý hồ sơ cá nhân)
  (Quản lý hồ sơ cá nhân) <.. (Cập nhật thông tin cá nhân) : <<include>>
  (Quản lý hồ sơ cá nhân) <.. (Cập nhật CV) : <<include>>
  (Quản lý hồ sơ cá nhân) <.. (Cập nhật kỹ năng) : <<include>>
  (Quản lý hồ sơ cá nhân) .> (Gợi ý tối ưu hồ sơ bằng AI) : <<extends>>
}

@enduml