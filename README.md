# Oni Ethereal Tarot

Trải nghiệm bói bài Tarot 3D huyền ảo trên nền web — tông đen tuyền, chữ trắng sáng — kết hợp điều khiển bằng cử chỉ tay (MediaPipe) và luận giải bằng AI (DeepSeek).

## ✨ Tính năng

- **🔮 Hình ảnh 3D huyền ảo**: bài được xếp theo hiệu ứng 3D dựng bằng CSS, nền đen tuyền cùng hiệu ứng hạt sáng trắng.
- **✋ Điều khiển bằng cử chỉ**: không cần chạm chuột, chỉ dùng camera.
  - **Vẫy tay hai bên**: cuộn dàn bài sang trái / phải.
  - **Nắm tay ở giữa màn hình**: chọn lá bài.
  - **Xòe năm ngón tay**: mở khóa luận giải định mệnh.
- **🤖 Luận giải bằng AI**: tích hợp DeepSeek API, luận giải theo phong cách huyền học và tâm lý học, trả về dạng streaming.
- **📱 Responsive**: tự động co giãn theo mọi kích thước màn hình.
- **🔒 Riêng tư**: dữ liệu camera chỉ xử lý cục bộ trên trình duyệt; API Key lưu trong `localStorage`, không đi qua máy chủ trung gian.

## 🚀 Chạy thử / Triển khai lên Vercel

Đây là ứng dụng single-file HTML, không cần bước build.

**Chạy cục bộ:**
```bash
python3 -m http.server 8000
```
Rồi mở `http://localhost:8000`.

**Triển khai lên Vercel:**
1. Đưa toàn bộ thư mục này (kèm `index.html` và `assets/`) lên một repo Git, hoặc dùng Vercel CLI:
   ```bash
   npm i -g vercel
   vercel
   ```
2. Vercel sẽ tự nhận diện đây là site tĩnh — không cần cấu hình build command hay output directory (để trống là được, vì `index.html` nằm ở thư mục gốc).

## 🎮 Hướng dẫn sử dụng

1. **Bắt đầu**: cho phép quyền camera, sau đó **xòe năm ngón tay và giữ 3 giây**.
2. **Chọn bài**:
   - Di chuyển tay sang **trái/phải** màn hình để cuộn dàn bài.
   - Khi lá bài mong muốn nằm giữa màn hình, **nắm tay và giữ 1 giây** để chọn.
   - Lặp lại để chọn đủ 3 lá (Quá khứ – Hiện tại – Tương lai).
3. **Luận giải bằng AI**: nhấn biểu tượng ⚙️ để nhập DeepSeek API Key, sau đó **xòe năm ngón tay giữ 3 giây** để nhận luận giải.

## 📚 Nguồn tài nguyên

Hình ảnh bộ bài Rider-Waite-Smith được lấy từ **[Sacred-Texts.com](https://sacred-texts.com/tarot/pkt/index.htm)** — *The Pictorial Key to the Tarot* của A.E. Waite, minh họa bởi Pamela Colman Smith (1911), thuộc phạm vi công cộng (public domain).

## 📄 Giấy phép

Dự án phát hành theo giấy phép [MIT License](LICENSE).
