```plantuml
@startuml
start
:Quản trị viên bắt đầu quản lý người dùng;
:Xem danh sách người dùng;
:Chọn người dùng cần quản lý;
if (Cập nhật thông tin?) then (yes)
  :Cập nhật thông tin người dùng;
  :Gửi thông tin cập nhật;
  :Hoàn tất cập nhật;
else (no)
  if (Khóa tài khoản?) then (yes)
    :Khóa tài khoản vi phạm;
    :Xác minh vi phạm;
    :Hoàn tất khóa tài khoản;
  else (no)
    :Quay lại danh sách người dùng;
  endif
endif
stop
@enduml