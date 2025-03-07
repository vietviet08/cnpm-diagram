@startuml
actor "Admin" as A
participant "Job Portal System" as JPS

A -> JPS: Quản lý công việc
JPS -> JPS: Xem danh sách công việc
A -> JPS: Gỡ bỏ công việc vi phạm
JPS -> JPS: Xác minh vi phạm
JPS -> A: Hoàn tất quản lý công việc

@enduml