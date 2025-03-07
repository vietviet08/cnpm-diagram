```plantuml
@startuml
|Người dùng|
start
: Bắt đầu đăng nhập;
: Nhập thông tin đăng nhập;
: Gửi thông tin đăng nhập;
|Job Portal System|
: Gửi mã xác thực hai lớp;
if (Mã xác thực đúng?) then (yes)
  : Xác thực thành công;
  : Đăng nhập hoàn tất;
  stop
else (no)
  : Mã xác thực sai;
  |Người dùng|
  if (Khôi phục mật khẩu?) then (yes)
    : Khôi phục mật khẩu thành công;
    : Quay lại bước nhập thông tin đăng nhập;
  else (no)
    : Đăng nhập thất bại;
    stop
  endif
endif
@enduml