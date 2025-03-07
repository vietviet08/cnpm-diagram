```plantuml
@startuml
start
:Nhà tuyển dụng bắt đầu quản lý lịch phỏng vấn;
:Xem danh sách lịch phỏng vấn;
:Chọn lịch phỏng vấn cần quản lý;
if (Cập nhật lịch?) then (yes)
  :Cập nhật lịch phỏng vấn;
  :Gửi thông tin cập nhật;
  :Hoàn tất quản lý lịch;
  stop
else (no)
  if (Hủy lịch?) then (yes)
    :Hủy lịch phỏng vấn;
    :Hoàn tất quản lý lịch;
    stop
  else (no)
    :Quay lại danh sách lịch;
    stop
  endif
endif
@enduml