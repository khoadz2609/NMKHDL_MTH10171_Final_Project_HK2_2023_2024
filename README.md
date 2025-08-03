# NMKHDL_MTH10171_Final_Project_HK2_2023_2024

## Giới thiệu

Đây là repository cho Đồ án cuối kỳ môn "Nhập môn Khoa học dữ liệu" (MTH10171) học kỳ 2 năm học 2023-2024. Dự án ứng dụng kỹ thuật crawling, tiền xử lý, phân tích dữ liệu và xử lý ngôn ngữ tự nhiên trên dữ liệu nhà đất được crawl từ web.

## Nội dung dự án

- **Tên đề tài:** [Dự đoán giá nhà]
- **Mô tả:**  
  Dự án thực hiện crawl dữ liệu nhà đất, tiền xử lý, ghép dữ liệu từ nhiều khu vực, sau đó áp dụng LLM (Large Language Model) để trích xuất thông tin từ trường mô tả tự do sang các trường có cấu trúc (giá nhà, diện tích, số phòng ngủ, số WC, địa chỉ, mặt tiền, số tầng...).  
  Ngoài ra còn thực hiện các task:
  - Tiền xử lý, ghép dữ liệu từ nhiều file csv crawl được (`Ghep_data.ipynb`).
  - Tách file lớn thành nhiều file nhỏ để xử lý song song với LLM (`LLM.ipynb`).
  - Sử dụng API Anyscale để trích xuất thông tin từ mô tả sang bảng có cấu trúc.
  - Ghép kết quả từ nhiều file nhỏ ra file hoàn chỉnh.

## Các file chính trong repo

- `.gitignore`: Loại trừ file `.env` (chứa biến môi trường, API key).
- `Crawling.ipynb`: Notebook crawl dữ liệu nhà đất từ web.
- `Ghep_data.ipynb`: Ghép các file csv crawl được thành một dataframe lớn, đổi tên cột, xuất ra file tổng hợp.
- `LLM.ipynb`: 
  - Đọc dữ liệu đã crawl, tách thành các file nhỏ để xử lý với LLM.
  - Sử dụng API Anyscale để trích xuất thông tin có cấu trúc từ mô tả bất động sản.
  - Ghép lại các file kết quả thành một file tổng hợp cuối cùng.
- `Preprocessing_and_FeatureEngineering.ipynb`: Tiến hành làm sạch dữ liệu, loại bỏ các giá trị ngoại lai ...
- `Methodology.ipynb`: Áp dụng các mô hình hồi quy.
- Thư mục `Data/`: Lưu dữ liệu (csv) crawl được.

## Cấu trúc thư mục

```
├── .gitignore
├── Crawling.ipynb
├── Data/
├── Ghep_data.ipynb
├── LLM.ipynb
├── Methodology.ipynb
├── Preprocessing_and_FeatureEngineering.ipynb
└── README.md
```
---
