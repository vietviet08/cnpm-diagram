```plantuml
@startuml
|Ứng viên|
start
: Bắt đầu nộp đơn xin việc;
: Chọn công việc;
: Đính kèm CV;
: Đính kèm thư xin việc;
if (Phân tích CV bằng AI?) then (yes)
  |Job Portal System|
  : Phân tích CV;
  : Hoàn tất nộp đơn;
  stop
else (no)
  : Hoàn tất nộp đơn;
  stop
endif
@enduml