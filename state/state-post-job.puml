@startuml
scale 350 width

[*] --> NhậpMôTả : Bắt đầu đăng tin tuyển dụng

state NhậpMôTả {
  [*] --> NhậpMôTảCôngViệc
  NhậpMôTảCôngViệc : Nhà tuyển dụng nhập mô tả công việc
  NhậpMôTảCôngViệc --> GửiMôTả : Nhập xong mô tả
  GửiMôTả : [*] --> KiểmDuyệt : Gửi mô tả công việc và yêu cầu
}

state KiểmDuyệt {
  [*] --> XácThựcThôngTin : Kiểm duyệt thông tin công ty
  XácThựcThôngTin --> ĐăngTinThànhCông : Xác thực thành công
}

KiểmDuyệt --> ĐăngTinThànhCông : Kiểm duyệt thành công
ĐăngTinThànhCông --> [*] : Tin tuyển dụng được đăng

@enduml