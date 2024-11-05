# Tự động tạo Nội Dung Tin Tức Đa Phương Tiện từ Văn Bản

## 1. Giới thiệu sản phẩm
Sản phẩm này là một hệ thống tự động chuyển đổi nội dung tin tức từ văn bản gốc thành các định dạng đa phương tiện bao gồm hình ảnh, âm thanh, và video. Thông qua các mô hình AI tiên tiến, hệ thống thực hiện quy trình sau:
- Tóm tắt văn bản để rút gọn nội dung nhưng vẫn giữ nguyên ý chính.
- Tạo hình ảnh từ văn bản để minh họa các đoạn tin tức.
- Chuyển đổi văn bản thành âm thanh để tạo trải nghiệm nghe.
- Kết hợp các thành phần hình ảnh, âm thanh và văn bản cuộn thành video tin tức hoàn chỉnh.
- Cuối cùng, tạo trang HTML hiển thị tin tức với hình ảnh và văn bản, cho phép tải xuống từng phần nội dung.

## 2. Công cụ và Thư viện sử dụng

### Công cụ chính:
- **MoviePy**: Thư viện Python mạnh mẽ hỗ trợ xử lý video để tạo video từ hình ảnh, văn bản và âm thanh.
- **CSS/HTML**: Dùng để tạo trang web hiển thị nội dung tin tức dưới dạng hình ảnh và văn bản minh họa.

### Mô hình AI:
- **BART** (facebook/bart-large-cnn): Mô hình dùng cho tóm tắt văn bản.
- **Stable Diffusion** (stabilityai/stable-diffusion-xl-base-1.0): Mô hình dùng để tạo hình ảnh từ văn bản.
- **Google Text-to-Speech (gTTS)**: Công cụ chuyển đổi văn bản thành giọng nói.

### Tính mới và Tính sáng tạo:
- **Tự động hóa đa phương tiện**: Sản phẩm tự động chuyển đổi văn bản thành nhiều định dạng đa phương tiện giúp người dùng tiếp cận tin tức một cách sinh động.
- **Hiệu ứng cuộn văn bản đồng bộ với âm thanh**: Kết hợp văn bản cuộn và giọng đọc đồng bộ, tạo trải nghiệm tin tức chuyên nghiệp và dễ theo dõi.
- **Ứng dụng linh hoạt**: Sản phẩm có thể mở rộng cho nhiều lĩnh vực như giáo dục, báo cáo doanh nghiệp, và nội dung quảng cáo.

## 3. Hướng dẫn cài đặt và chạy code
### Bước 1: Chạy mã nguồn chính

- **Tóm tắt văn bản**: Mã nguồn sẽ đọc tệp JSON đầu vào chứa nội dung tin tức, sử dụng mô hình BART để tóm tắt các câu và ghép lại thành nội dung rút gọn.
  
- **Tạo hình ảnh từ văn bản**: Với mỗi câu tóm tắt, hệ thống sẽ sử dụng Stable Diffusion để tạo hình ảnh minh họa và lưu các ảnh này vào thư mục `images`.
  
- **Chuyển văn bản thành âm thanh**: Mỗi đoạn văn bản sẽ được chuyển thành âm thanh bằng gTTS và lưu vào thư mục `audio_clips`.
  
- **Tạo video từ hình ảnh, âm thanh, và văn bản**: Hệ thống kết hợp hình ảnh, văn bản cuộn, và âm thanh thành các đoạn video clip và nối lại thành video hoàn chỉnh.
  
- **Tạo trang HTML hiển thị tin tức**: Trang HTML hiển thị toàn bộ nội dung tin tức, hình ảnh và văn bản, cho phép người dùng tải xuống từng phần.

### Bước 2: Kiểm tra và tải xuống kết quả

- **Video**: Video được tạo sẽ lưu dưới tên `final_news_video_v1.mp4`.
- **HTML**: Trang HTML được tạo sẽ lưu dưới tên `news_report.html`.
- **Tải xuống các nội dung**: Sau khi thực hiện xong, bạn có thể tải về các tệp hình ảnh, âm thanh và video thông qua Colab.

## 4. Hướng dẫn sử dụng sản phẩm

1. **Cung cấp văn bản tin tức**: Đưa tệp JSON chứa nội dung tin tức vào thư mục đầu vào. Tệp JSON này sẽ chứa các đoạn tin tức mà bạn muốn tóm tắt và chuyển đổi thành nội dung đa phương tiện.

2. **Chạy code**: Thực hiện các bước cài đặt và chạy mã nguồn theo hướng dẫn ở các phần trước. Mã nguồn sẽ tự động thực hiện các bước:
   - Tóm tắt văn bản tin tức.
   - Tạo hình ảnh minh họa từ nội dung tóm tắt.
   - Chuyển đổi văn bản thành giọng nói.
   - Kết hợp hình ảnh, văn bản và âm thanh để tạo thành video hoàn chỉnh.

3. **Xem kết quả**:
   - **Trang HTML**: Sau khi chạy xong, trang HTML sẽ hiển thị tin tức với từng hình ảnh và văn bản tương ứng. Mỗi mục tin tức có thể xem và tải xuống riêng lẻ.
   - **Video**: Video tin tức tự động tạo, bao gồm hiệu ứng cuộn văn bản, hình ảnh minh họa, và âm thanh giọng đọc.

4. **Tải xuống nội dung**: Bạn có thể tải về từng tệp hình ảnh, âm thanh và video để sử dụng hoặc chia sẻ.

## 5. Lợi ích của sản phẩm

- **Tiết kiệm thời gian**: Tự động hóa toàn bộ quy trình tạo nội dung đa phương tiện từ văn bản, giúp tiết kiệm thời gian biên tập và trình bày tin tức.
  
- **Trải nghiệm đa phương tiện**: Sản phẩm cung cấp trải nghiệm tin tức sống động, dễ tiếp cận qua các định dạng hình ảnh, âm thanh và video, phù hợp với người dùng có nhu cầu truy cập tin tức nhanh chóng và trực quan.

- **Tùy chỉnh và mở rộng dễ dàng**: Cấu trúc của sản phẩm cho phép tùy chỉnh và mở rộng để phục vụ cho nhiều lĩnh vực khác nhau như giáo dục, trợ lý ảo, và báo cáo kinh doanh. Sản phẩm có thể điều chỉnh để phù hợp với từng mục đích sử dụng.

## 6. Liên hệ và hỗ trợ

Nếu bạn gặp vấn đề hoặc cần thêm hỗ trợ, vui lòng liên hệ với nhóm phát triển qua email: [22028116@vnu.edu.vn]

---
