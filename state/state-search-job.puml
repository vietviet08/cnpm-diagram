@startuml
scale 350 width

[*] --> ChọnTiêuChí : Bắt đầu tìm kiếm công việc

state ChọnTiêuChí {
  [*] --> NhậpTiêuChí
  NhậpTiêuChí : Người dùng nhập tiêu chí tìm kiếm
  NhậpTiêuChí --> GửiTiêuChí : Nhập xong tiêu chí
  GửiTiêuChí : [*] --> LọcKếtQuả : Gửi tiêu chí
}

state LọcKếtQuả {
  [*] --> PhânTíchTiêuChí : Phân tích tiêu chí
  PhânTíchTiêuChí --> HiểnThịKếtQuả : Hiển thị kết quả
}

LọcKếtQuả --> PhânTíchHồSơ : [*] : Lọc kết quả

state PhânTíchHồSơ {
  [*] --> PhânTíchBằngAI
  PhânTíchBằngAI : Phân tích hồ sơ bằng AI
  PhânTíchBằngAI --> GợiÝViệcLàm : Gợi ý việc làm
}

PhânTíchHồSơ --> HiểnThịKếtQuả : Phân tích xong

HiểnThịKếtQuả --> [*] : Hiển thị kết quả tìm kiếm

@enduml