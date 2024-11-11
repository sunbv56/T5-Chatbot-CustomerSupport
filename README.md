# T5-Chatbot-CustomerSupport
Developed a customer support chatbot using the T5 model, fine-tuned to handle common queries with natural language processing, providing accurate and efficient responses to enhance user experience.
---

# T5 Chatbot for Customer Support

Dự án này triển khai một chatbot hỗ trợ khách hàng sử dụng mô hình T5 fine-tuned, nhằm trả lời các câu hỏi phổ biến của khách hàng. Dự án bao gồm mã nguồn fine-tune mô hình T5 và giao diện web để triển khai chatbot. Mô hình đã được huấn luyện trên Kaggle với 2 GPU và đã được upload công khai lên Hugging Face. Giao diện web sử dụng API của Hugging Face để gửi yêu cầu từ HTML và nhận phản hồi từ mô hình.

## Mô tả Dự án

Dự án bao gồm hai phần chính:

1. **Fine-tuning T5 Model**: Tệp `t5-chatbot-bitext-gen-ai-chatbot-customer-support.ipynb` chứa mã nguồn để fine-tune mô hình T5. Mô hình này được huấn luyện để có thể trả lời các câu hỏi hỗ trợ khách hàng một cách tự nhiên và chính xác. Mô hình được huấn luyện trên Kaggle với sự hỗ trợ của 2 GPU.

2. **Triển khai Giao diện Web**: Tệp `index.html` cung cấp giao diện người dùng đơn giản cho chatbot, giúp người dùng dễ dàng tương tác với chatbot qua web. Giao diện web này sử dụng API của Hugging Face để gửi các yêu cầu từ HTML và nhận phản hồi từ mô hình đã được huấn luyện.

## Cấu trúc Dự án

- **t5-chatbot-bitext-gen-ai-chatbot-customer-support.ipynb**:
  - Tiền xử lý dữ liệu huấn luyện.
  - Fine-tuning mô hình T5 trên dữ liệu hỗ trợ khách hàng.
  - Lưu trữ mô hình đã được huấn luyện để sử dụng cho chatbot.

- **index.html**:
  - Giao diện người dùng giúp người dùng tương tác với chatbot trên nền tảng web thông qua API của Hugging Face.

## Cài đặt Môi trường

1. **Clone repository**:
   ```bash
   git clone https://github.com/sunbv56/T5-Chatbot-CustomerSupport.git
   cd T5-Chatbot-CustomerSupport
   ```

2. **Cài đặt các thư viện yêu cầu**:
   Sau khi tạo môi trường ảo, bạn có thể cài đặt các thư viện cần thiết bằng lệnh sau:

   ```bash
   pip install -r requirements.txt
   ```

## Huấn luyện Mô hình

1. **Mở tệp `t5-chatbot-bitext-gen-ai-chatbot-customer-support.ipynb`**:
   - Sử dụng Jupyter Notebook hoặc Google Colab để mở và chạy notebook.
   - Notebook này hướng dẫn bạn cách fine-tune mô hình T5 với dữ liệu hỗ trợ khách hàng.
   - Mô hình đã được huấn luyện trên Kaggle với 2 GPU và kết quả đã được upload lên Hugging Face để có thể sử dụng công khai.

2. **Chạy toàn bộ notebook** để huấn luyện mô hình:
   - Từ bước tiền xử lý dữ liệu đến fine-tuning mô hình.
   - Sau khi mô hình được huấn luyện, mô hình sẽ được lưu trữ.

## Triển khai Giao diện Web

1. **Chạy Giao diện Web**:
   - Sau khi fine-tune mô hình, bạn có thể sử dụng tệp `index.html` để triển khai giao diện chatbot trên web.
   - Giao diện web này sử dụng API của Hugging Face để gửi yêu cầu từ HTML và nhận phản hồi từ mô hình đã được huấn luyện.

2. **Gửi yêu cầu từ HTML**:
   - Giao diện web sẽ gọi API từ Hugging Face để tương tác với mô hình và nhận phản hồi cho người dùng.

## Các Thư viện Được Sử Dụng

- **evaluate**: Đánh giá hiệu suất mô hình.
- **sentence_transformers**: Dùng để trích xuất đặc trưng câu cho các tính toán độ tương đồng.
- **faiss-cpu**: Dùng để tìm kiếm tương đồng trong không gian vector.
- **rouge_score**: Đánh giá chất lượng của câu trả lời được sinh ra.
- **bert-score**: Đánh giá độ chính xác giữa văn bản sinh ra và văn bản tham chiếu.
- **transformers**: Thư viện chính để sử dụng mô hình T5.
- **torch**: Thư viện tính toán cho các mô hình học sâu.
- **matplotlib, seaborn**: Dùng để vẽ biểu đồ trực quan trong quá trình phân tích và đánh giá mô hình.

## Đóng góp

Mọi đóng góp đều được hoan nghênh! Nếu bạn phát hiện lỗi, có đề xuất cải tiến hoặc muốn thêm tính năng mới, vui lòng tạo một issue hoặc gửi pull request.

---
