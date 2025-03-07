@startuml

entity "users" as users {
  id: integer <<PK>>
  user_code: string
  username: string
  password: string
  created_at: timestamp
  updated_at: timestamp
}

entity "profiles" as profiles {
  id: integer <<PK>>
  user_id: integer
  fullname: string
  day_of_birth: date
  email: string
  phone_number: string
  created_at: timestamp
  updated_at: timestamp
}

entity "roles" as roles {
  id: integer <<PK>>
  slug: string
  description: string
  role: string
}

entity "role_user" as role_user {
  id: integer <<PK>>
  user_id: integer
  role_id: integer
}

entity "jobs" as jobs {
  id: integer <<PK>>
  company_id: integer
  title: string
  description: string
  location: string
  salary: decimal
  status: enum('open', 'closed')
  category_id: integer
  job_type: enum("full-time", "part-time", "internship", "contract")
  created_at: timestamp
  updated_at: timestamp
}

entity "categories" as categories {
  id: integer <<PK>>
  category_name: string
  slug: string
  description: string
}

entity "applies" as applies {
  id: integer <<PK>>
  user_id: integer
  job_id: integer
  status: string
  apply_date: date
  cv_id: integer
}

entity "companies" as companies {
  id: integer <<PK>>
  user_id: integer
  avatar_url: string
  company_name: string
  introduce: string
  address: string
  slug: string
}

entity "cvs" as cvs {
  id: integer <<PK>>
  cv_img: string
  user_id: integer
  is_default: bool
  created_at: timestamp
  updated_at: timestamp
}

entity "posts" as posts {
  id: integer <<PK>>
  title: string
  user_id: integer
  created_at: timestamp
  updated_at: timestamp
}

entity "group_chat" as group_chat {
  id: integer <<PK>>
  group_avatar: string
  description: string
  last_interact: date
}

entity "chat_members" as chat_members {
  id: integer <<PK>>
  user_id: integer
  group_chat_id: integer
  join_date: date
}

entity "messages" as messages {
  id: integer <<PK>>
  group_chat_id: string
  sender_id: integer
  receiver_id: integer
  message: string
  send_date: date
}

users ||--o{ profiles : "id - user_id"
profiles ||--|| users : "user_id - id"
users ||--o{ role_user : "id - user_id"
roles ||--o{ role_user : "id - role_id"
role_user }o--|| users : "role_id - id"
jobs ||--o{ categories : "category_id - id"
categories ||--o| jobs : "id - category_id"
companies ||--o{ jobs : "id - company_id"
jobs ||--o{ applies : "id - job_id"
applies ||--|| cvs : "cv_id - id"
companies ||--o{ applies : "id - company_id"
users ||--o{ cvs : "id - user_id"
users ||--o{ applies : "id - user_id"
users ||--o{ posts : "id - user_id"
chat_members ||--|| users : "user_id - id"
chat_members ||--|| group_chat : "group_chat_id - id"
group_chat ||--o{ messages : "id - group_chat_id"
messages ||--|| users : "sender_id - id"
messages ||--|| users : "receiver_id - id"

@enduml
