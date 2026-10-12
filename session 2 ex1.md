

| STT | Phương thức | Endpoint | Mô tả | Request Body / Query |
| 1 | `GET` | `/tasks` | Lấy danh sách toàn bộ công việc | Không có |
| 2 | `GET` | `/users` | Lấy danh sách toàn bộ người dùng | Không có |
| 3 | `POST` | `/tasks` | Tạo mới một công việc | `{ "title": "...", "priority": "high" }` |
| 4 | `POST` | `/users` | Tạo mới một người dùng | `{ "username": "...", "role": "USER" }` |
| 5 | `PATCH` | `/tasks/{id}/status` | Cập nhật trạng thái công việc | `{ "status": "COMPLETED" }` |
| 6 | `PATCH` | `/users/{id}/role` | Cập nhật vai trò người dùng | `{ "role": "ADMIN" }` |
| 7 | `DELETE` | `/tasks/{id}` | Xóa một công việc | Không có |
| 8 | `DELETE` | `/users/{id}` | Xóa một người dùng | Không có |
| 9 | `GET` | `/tasks?priority=high` | Lọc công việc có độ ưu tiên high | `priority=high` |
| 10 | `GET` | `/users/{userId}/tasks?priority=high` | Công việc ưu tiên high của user cụ thể | `priority=high` |
| 11 | `GET` | `/users/{userId}/tasks` | Liệt kê toàn bộ công việc của 1 user | Không có |
| 12 | `PATCH` | `/tasks/{id}/assign` | Gắn công việc cho người dùng | `{ "userId": 1 }` |