```plantuml
@startuml
start
:Người dùng bắt đầu đăng ký;
:Nhập thông tin cá nhân;
if (Thông tin hợp lệ?) then (yes)
  :Gửi thông tin;
  :Gửi email xác thực;
  if (Email xác thực thành công?) then (yes)
    :Gợi ý tối ưu hồ sơ bằng AI;
    :Hồ sơ tối ưu thành công;
    :Đăng ký hoàn tất;
    stop
  else (no)
    :Email xác thực thất bại;
    :Người dùng nhập lại thông tin;
    :Quay lại bước nhập thông tin cá nhân;
  endif
else (no)
  :Thông tin không hợp lệ;
  :Quay lại bước nhập thông tin cá nhân;
endif
@enduml