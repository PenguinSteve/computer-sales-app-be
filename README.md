-   Mở terminal ở thư mục chứa file docker-compose.yml
-   Chạy câu lệnh: docker compose up -d --build
-   Có thể tùy chỉnh port trong file docker-compose.yml và Dockerfile

Công nghệ sử dụng
* Node.js: môi trường runtime JavaScript không đồng bộ, phù hợp xây dựng server backend mạnh mẽ, mở rộng cao; triển khai trên Google Cloud
* REST API: giao tiếp giữa frontend và backend qua HTTP (GET, POST, PUT, DELETE) để xử lý dữ liệu
* Socket.IO: thư viện giao tiếp hai chiều, thời gian thực giữa client và server, dùng cho tính năng bình luận/đánh giá ngay lập tức, chat realtime giữa user và admin
* Redis: lưu trữ in‑memory, dùng làm message broker cho hàng đợi gửi email; một worker xử lý nền kéo email từ Redis và thực hiện gửi
* Elasticsearch: công cụ tìm kiếm dựa trên Lucene, cung cấp tìm kiếm nhanh, gợi ý và khớp gần đúng cho sản phẩm
