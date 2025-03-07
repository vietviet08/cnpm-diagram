```plantuml
@startuml
start
:Ứng viên bắt đầu quản lý hồ sơ cá nhân;
:Cập nhật thông tin cá nhân;
:Nhập thông tin cá nhân;
:Gửi thông tin;
:Cập nhật CV;
:Nhập CV;
:Gửi CV;
:Cập nhật kỹ năng;
:Nhập kỹ năng;
:Gửi kỹ năng;
if (Tối ưu hồ sơ bằng AI?) then (yes)
  :Phân tích hồ sơ;
  :Hồ sơ tối ưu;
  stop
else (no)
  :Hoàn tất quản lý hồ sơ;
  stop
endif
@enduml