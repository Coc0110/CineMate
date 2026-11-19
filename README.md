# CineMate — App Cộng đồng Đánh giá Phim & Lịch chiếu tích hợp Chatbot AI

Dự án tích hợp 3 học phần:
- Quản lý dự án Công nghệ thông tin (MAN104)
- Cơ sở dữ liệu nâng cao
- Lập trình trên thiết bị di động

## Cấu trúc Monorepo
- [`/backend`](backend/README.md): REST API, Swagger/OpenAPI, xác thực & phân quyền (3 vai trò), tích hợp Chatbot AI (LLM + Tool Calling + Log).
- [`/mobile`](mobile/README.md): Ứng dụng di động (Android APK) cho người dùng cuối.
- [`/admin-web`](admin-web/README.md): Web quản trị & kiểm duyệt nội dung, dashboard thống kê.
- [`/database`](database/README.md): Thiết kế ERD (≥ 8 bảng), script DDL, Index, Trigger, Stored Procedure, Materialized View, Seed data.
- [`/docs`](docs/README.md): Hồ sơ quản lý dự án (D01–D27), Test Cases (≥ 30 câu hỏi chatbot), biên bản khảo sát & UAT.

## Quy ước Gitflow & Commit
- `main`: Nhánh phát hành ổn định (tag `v0.1`, `v0.2`, `v1.0`).
- `develop`: Nhánh tích hợp chính.
- `feature/CM-<id>-<mo-ta>`: Tách từ `develop`, tạo PR vào `develop`.
- Format commit: `[CM-<id>] <type>: <mô tả ngắn>` (ví dụ: `[CM-1] chore: init monorepo structure`).
