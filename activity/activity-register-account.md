```plantuml
@startuml
|Người dùng|
start
: Bắt đầu đăng ký;
: Nhập thông tin cá nhân;
: Gửi thông tin;
|Job Portal System|
: Gửi email xác thực;
if (Email xác thực thành công?) then (yes)
  : Gợi ý tối ưu hồ sơ bằng AI;
  : Hồ sơ tối ưu thành công;
  : Đăng ký hoàn tất;
  stop
else (no)
  : Email xác thực thất bại;
  : Người dùng nhập lại thông tin;
  : Quay lại bước nhập thông tin cá nhân;
endif
@enduml