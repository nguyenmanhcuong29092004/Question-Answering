# Xây dựng hệ thống hỏi-đáp mở với hệ cơ sở dữ liệu vector

## Giới thiệu

Dự án này nhằm phát triển một hệ thống hỏi-đáp tự động với khả năng trả lời các câu hỏi dựa trên nội dung từ các đoạn văn bản. Hệ thống được chia thành hai phần chính: **Retriever** và **Reader**.

- **Retriever**: Truy xuất các đoạn văn bản có liên quan từ một cơ sở dữ liệu vector.
- **Reader**: Đọc đoạn văn bản được truy xuất và đưa ra câu trả lời tương ứng.

Dự án được triển khai trên bộ dữ liệu **SQuAD 2.0** (Stanford Question Answering Dataset), một bộ dữ liệu chuẩn trong lĩnh vực hỏi-đáp.

## Cấu trúc dự án

- `Reader_QA.ipynb`: Notebook hướng dẫn huấn luyện và sử dụng mô hình trả lời câu hỏi.
- `retriever_and_demo.py`: Script thực hiện việc truy xuất và trả lời câu hỏi từ dữ liệu đã được index bằng Faiss. Sau đó sẽ demo bằng streamlit.
- `README.md`: Tài liệu này cung cấp thông tin chi tiết về dự án và cách sử dụng.

## Yêu cầu hệ thống

- Python 3.7 hoặc cao hơn
- Các thư viện Python cần thiết:
  - `transformers`
  - `datasets`
  - `torch`
  - `numpy`
  - `faiss-gpu`
  - `tqdm`

## Hướng dẫn cài đặt

1. **Clone dự án từ GitHub**:
   ```bash
   git clone <repo_url>
   cd <project_directory>
2. **Chạy trên môi trường anaconda**
   ```bash
   conda activate <username>
   streamlit run retriever_and_demo.py


