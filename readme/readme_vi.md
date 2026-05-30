# VK Video Parser Tool 🎬

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Language](https://img.shields.io/badge/language-Tiếng_Việt-yellow.svg)

## 📋 Tổng Quan Dự Án

**VK Video Parser Tool** là công cụ hỗ trợ dựa trên nền web, được thiết kế để hỗ trợ nhà giáo dục, nhà nghiên cứu và người học cá nhân trong việc phân tích kỹ thuật các nội dung video có thể truy cập công khai trên nền tảng VK, dưới nguyên tắc "sử dụng hợp lý" (Fair Use). Mục tiêu của công cụ là hỗ trợ lưu trữ nội dung cho mục đích giáo dục, nghiên cứu và học tập cá nhân. Công cụ này tập trung cung cấp hỗ trợ kỹ thuật đơn giản, hiệu quả cho các kịch bản phi thương mại như thu thập trường hợp giảng dạy, nghiên cứu truyền thông xã hội, phân tích văn hóa khu vực và quản lý kiến thức cá nhân.

🔗 **Truy Cập Trực Tuyến**: [https://twittervideodownloaderx.com/vk_downloader_vi](https://twittervideodownloaderx.com/vk_downloader_vi)

> ⚠️ **Thông Báo Quan Trọng**: Dự án này chỉ được phát triển cho mục đích học tập kỹ thuật và nghiên cứu. Người dùng được kỳ vọng sẽ tuân thủ luật bản quyền và điều khoản dịch vụ của nền tảng liên quan, tôn trọng quyền của tác giả gốc, và tuyệt đối không sử dụng công cụ này cho bất kỳ hoạt động nào xâm phạm sở hữu trí tuệ hoặc vi phạm chính sách nền tảng.

---

## ✨ Tính Năng Chính

- 🔗 **Nhận Diện Liên Kết Thông Minh**: Tự động phân tích liên kết trang video VK, liên kết nhúng và nhiều định dạng khác
- 📥 **Hỗ Trợ Tùy Chọn Chất Lượng**: Hiển thị độ phân giải khả dụng dựa trên siêu dữ liệu nguồn (theo thông tin công khai của nền tảng)
- 📱 **Tương Thích Đa Thiết Bị**: Thiết kế phản hồi tối ưu cho cả trình duyệt máy tính để bàn và thiết bị di động
- 🔐 **Ưu Tiên Quyền Riêng Tư**: Không ghi nhật ký hoạt động người dùng, không lưu trữ nội dung đã phân tích trên máy chủ
- ⚡ **Nhẹ Và Nhanh**: Logic xử lý tập trung vào phía client, giảm phụ thuộc máy chủ, phản hồi nhanh chóng
- 🔄 **Bảo Trì Liên Tục**: Cập nhật thường xuyên để thích ứng với thay đổi frontend của nền tảng, duy trì khả năng sử dụng của công cụ
- 💬 **Trích Xuất Siêu Dữ Liệu**: Tùy chọn trích xuất thông tin công khai như tiêu đề video, người tải lên, album (chỉ cho mục đích ghi chú nghiên cứu)

---

## 🚀 Hướng Dẫn Sử Dụng

### Bước 1: Sao Chép Liên Kết Video
1. Mở trang web hoặc ứng dụng VK
2. Tìm **nội dung video công khai** mà bạn muốn phân tích
3. Nhấn "Chia sẻ" → "Sao chép liên kết" hoặc sao chép trực tiếp URL trang video từ thanh địa chỉ trình duyệt

### Bước 2: Gửi Yêu Cầu Phân Tích
1. Truy cập trang công cụ: `https://twittervideodownloaderx.com/vk_downloader_vi`
2. Dán liên kết đã sao chép vào trường nhập liệu được cung cấp
3. Nhấp nút "Bắt Đầu Phân Tích"

### Bước 3: Xem Kết Quả
1. Đợi hệ thống hoàn thành phân tích kỹ thuật (thường chỉ vài giây)
2. Xem trước siêu dữ liệu video và thông tin khả dụng
3. Thực hiện các bước tiếp theo theo hướng dẫn (chỉ dành cho mục đích học tập cá nhân)

---

## 💡 Ví Dụ Liên Kết Được Hỗ Trợ

```
✅ Định dạng URL được khuyến nghị:
- https://vk.com/video-xxxxx_xxxxx
- https://vk.com/video_xxxxx_xxxxx
- https://vk.com/clip-xxxxx_xxxxx
- https://m.vk.com/video-xxxxx_xxxxx (liên kết phiên bản di động)

❌ Trường hợp hiện không được hỗ trợ:
- Video được đặt ở chế độ "Chỉ bạn bè" hoặc "Riêng tư"
- Nội dung yêu cầu xác thực đăng nhập để truy cập
- Video được bảo vệ bởi hệ thống quản lý quyền kỹ thuật số (DRM) nâng cao
- Nội dung vi phạm hướng dẫn cộng đồng của VK
- Video đã xóa hoặc bị giới hạn khu vực
```

---

## ⚙️ Kiến Trúc Kỹ Thuật

| Thành Phần | Triển Khai | Mô Tả |
|-----------|-----------|-------|
| **Frontend** | HTML5 + CSS3 + Vanilla JS | Không phụ thuộc framework, tải nhanh, tương thích cao |
| **Xử Lý Yêu Cầu** | Node.js / Python Backend | Bất đồng bộ không chặn, hỗ trợ xử lý song song cao, vận hành ổn định |
| **Phân Tích Nội Dung** | Biểu Thức Chính Quy + Phân Tích DOM + VK API | Chỉ trích xuất siêu dữ liệu công khai, không vượt qua mã hóa, tôn trọng quyền truy cập |
| **Lớp Bảo Mật** | HTTPS + Lọc Đầu Vào + Giới Hạn Tốc Độ | Ngăn chặn lạm dụng, đảm bảo ổn định dịch vụ, bảo vệ quyền riêng tư người dùng |
| **Môi Trường Triển Khai** | Docker + Tăng Tốc CDN | Phân tán node toàn cầu, truy cập độ trễ thấp, mở rộng linh hoạt |

---

## ⚠️ Tuyên Bố Tuân Thủ Và Sử Dụng Có Trách Nhiệm

Công cụ này hoạt động nghiêm ngặt theo nguyên tắc **trung lập kỹ thuật** và **sử dụng hợp lý**. Vui lòng tuân thủ các hướng dẫn sau:

### ✅ Trường Hợp Sử Dụng Được Phép
- 📚 Cơ sở giáo dục phân tích trường hợp lan truyền trên mạng xã hội khu vực cho nghiên cứu học thuật
- 🔬 Dự án nghiên cứu liên quan đến lấy mẫu, ghi chú và nghiên cứu văn hóa nội dung video khu vực
- 🗂️ Nhà nghiên cứu cá nhân sắp xếp tài liệu tham khảo để lấy cảm hứng (với ghi nguồn phù hợp)
- 🌐 Truy cập nội dung ngoại tuyến cho mục đích học tập ở khu vực có kết nối internet hạn chế
- 📊 Quan sát và ghi chép hiện tượng văn hóa mạng vì mục đích phi thương mại

### ❌ Hành Vi Bị Cấm
- 🚫 Sử dụng nội dung đã phân tích để phân phối thương mại, tái phát hành thứ cấp hoặc kiếm tiền từ lưu lượng truy cập
- 🚫 Xóa thông tin tác giả gốc hoặc watermark và đăng lại nội dung như tác phẩm gốc
- 🚫 Thu thập dữ liệu hàng loạt, thu thập dữ liệu tự động hoặc làm gián đoạn hoạt động của VK
- 🚫 Cố gắng vượt qua kiểm soát truy cập để xem nội dung không công khai hoặc bị hạn chế
- 🚫 Sử dụng để lan truyền nội dung vi phạm pháp luật, xâm phạm quyền hoặc vi phạm hướng dẫn cộng đồng

### 📜 Khung Tham Chiếu Pháp Lý
- Luật Sở hữu trí tuệ Việt Nam và các quy định về sử dụng hợp lý, trích dẫn
- Luật An ninh mạng và các quy định liên quan đến bảo vệ dữ liệu cá nhân
- Điều khoản dịch vụ và Hướng dẫn cộng đồng của nền tảng VK
- Nguyên tắc tư pháp quốc tế được công nhận về "sử dụng hợp lý" (Fair Use)

> 📌 **Tuyên Bố Miễn Trừ Trách Nhiệm**: Nhà phát triển không chịu trách nhiệm cho bất kỳ hậu quả nào do việc sử dụng sai mục đích công cụ này. Bằng cách sử dụng phần mềm này, bạn xác nhận rằng bạn đã đọc, hiểu và đồng ý tuân thủ các điều khoản nêu trên.

---

## 🤝 Hướng Dẫn Đóng Góp

Chúng tôi hoan nghênh sự đóng góp từ cộng đồng để giúp cải thiện dự án này:

```bash
# 1. Fork repository này
# 2. Tạo branch tính năng mới
git checkout -b feature/improvement

# 3. Commit các thay đổi của bạn
git commit -m "feat: cải thiện logic nhận diện liên kết VK"

# 4. Push và mở Pull Request
git push origin feature/improvement
```

**Hướng Dẫn Đóng Góp**:
- Tuân thủ quy tắc kiểu mã ESLint / Prettier
- Bao gồm kiểm thử đơn vị cho chức năng mới khi có thể
- Sử dụng message commit rõ ràng, mô tả được (tiếng Việt hoặc tiếng Anh)
- Tài liệu hóa tính năng mới cả trong chú thích mã và cập nhật README
- Đảm bảo bản nộp vượt qua kiểm tra mã cơ bản trước khi gửi

---

## 🐛 Báo Cáo Vấn Đề

Nếu phát hiện lỗi hoặc có đề xuất cải tiến:

1. Kiểm tra tab [Issues](../../issues) trước để tránh báo cáo trùng lặp
2. Khi tạo issue mới, vui lòng bao gồm các thông tin sau:
   - Tên và phiên bản trình duyệt
   - Các bước tái hiện vấn đề (theo từng bước)
   - Hành vi mong đợi và hành vi thực tế
   - Ảnh chụp màn hình hoặc log lỗi (nếu có)
   - Ví dụ liên kết video VK (đã xử lý ẩn thông tin nhạy cảm)
3. Nhóm sẽ xem xét các lượt gửi định kỳ và phản hồi sớm nhất có thể

---

## 📄 Giấy Phép

Dự án này được phân phối dưới **Giấy phép MIT**. Bạn có thể tự do sử dụng, sửa đổi và phân phối phần mềm này, với điều kiện phải giữ nguyên thông báo bản quyền gốc và các điều khoản giấy phép.

```
MIT License

Copyright (c)  VK Video Parser Project

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Lời Cảm Ơn

- Xin cảm ơn cộng đồng nguồn mở đã cung cấp các thành phần kỹ thuật mạnh mẽ và nguồn cảm hứng
- Trân trọng cảm ơn người dùng và nhà nghiên cứu học thuật đã đóng góp phản hồi giá trị
- Tôn vinh những người sáng tạo nội dung trên VK đã làm phong phú giá trị nội dung văn hóa số

---

> 📬 **Hỗ Trợ Và Liên Hệ**: Đối với các câu hỏi về hợp tác kỹ thuật hoặc vấn đề tuân thủ, vui lòng gửi ticket qua GitHub Issues. Chúng tôi sẽ nỗ lực phản hồi các yêu cầu chính đáng một cách nhanh chóng.

*Dự án này không liên kết, được tài trợ hoặc phê duyệt chính thức bởi VK.com hoặc bất kỳ công ty liên kết nào. Tất cả nhãn hiệu, logo và tên thương hiệu là tài sản của chủ sở hữu tương ứng. Công cụ này chỉ cung cấp hỗ trợ phân tích kỹ thuật thuần túy và không thực hiện lưu trữ, phân phối hoặc tuyên bố quyền sở hữu đối với nội dung của bên thứ ba.*