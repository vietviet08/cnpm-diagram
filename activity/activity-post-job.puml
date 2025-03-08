```plantuml
@startuml
|Nhà tuyển dụng|
start
: Bắt đầu đăng tin tuyển dụng;
: Nhập mô tả công việc;
if (Mô tả hợp lệ?) then (yes)
  : Gửi mô tả công việc;
  : Nhập yêu cầu công việc;
  if (Yêu cầu hợp lệ?) then (yes)
    : Gửi yêu cầu công việc;
    |Job Portal System|
    : Kiểm duyệt tin tuyển dụng;
    if (Xác thực thông tin công ty?) then (yes)
      : Đăng tin thành công;
      stop
    else (no)
      : Xác thực thất bại;
      : Quay lại bước nhập thông tin công việc;
    endif
  else (no)
    : Yêu cầu không hợp lệ;
    : Quay lại bước nhập yêu cầu công việc;
  endif
else (no)
  : Mô tả không hợp lệ;
  : Quay lại bước nhập mô tả công việc;
endif
@enduml