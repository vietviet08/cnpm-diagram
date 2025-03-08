```plantuml
@startuml
start
:Nhà tuyển dụng bắt đầu quản lý tin tuyển dụng;
:Xem danh sách tin tuyển dụng;
:Chọn tin tuyển dụng cần quản lý;
if (Cập nhật tin?) then (yes)
  :Cập nhật tin tuyển dụng;
  :Gửi tin cập nhật;
  :Hoàn tất quản lý tin;
  stop
else (no)
  if (Xóa tin?) then (yes)
    :Xóa tin tuyển dụng;
    :Hoàn tất quản lý tin;
    stop
  else (no)
    :Quay lại danh sách tin;
    stop
  endif
endif
@enduml