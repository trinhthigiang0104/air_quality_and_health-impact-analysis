# 🌿 Air Quality and Health Impact Analysis (2015-2025)

## 📌 Tổng quan dự án (Project Overview)
Dự án này tập trung nghiên cứu mối liên hệ phức tạp giữa biến đổi khí hậu, ô nhiễm không khí và các rủi ro sức khỏe cộng đồng trên phạm vi toàn cầu. Bằng cách phân tích dữ liệu lịch sử từ 2015-2025, dự án xây dựng mô hình dự báo tỷ lệ bệnh tật, hỗ trợ các tổ chức y tế đưa ra quyết định dựa trên dữ liệu.

* **Vấn đề:** Mức độ tác động cụ thể của từng chỉ số môi trường (PM2.5, nhiệt độ cực đoan) đến sức khỏe con người.
* **Mục tiêu:** Xây dựng mô hình Machine Learning dự báo tỷ lệ bệnh hô hấp và tử vong do tim mạch dựa trên các biến số môi trường và kinh tế xã hội.

## 🛠 Công cụ & Thư viện (Tech Stack)
* **Ngôn ngữ:** Python 3.x
* **Phân tích & Xử lý:** `Pandas`, `NumPy`
* **Trực quan hóa:** `Matplotlib`, `Seaborn`, `Folium` (Bản đồ nhiệt địa lý)
* **Machine Learning:** `Scikit-learn`, `XGBoost`
* **Môi trường:** Jupyter Notebook / Google Colab

## 📊 Quy trình triển khai (Project Roadmap)
1.  **Tiền xử lý dữ liệu:** Làm sạch dữ liệu với 14,100 bản ghi, xử lý giá trị thiếu và chuẩn hóa 30 biến số.
2.  **Phân tích khám phá (EDA):** Trực quan hóa xu hướng theo mùa (Seasonality) và mối tương quan giữa khí hậu với chất lượng không khí.
3.  **Xây dựng mô hình:** Thử nghiệm các mô hình Regression (Random Forest, XGBoost) và tối ưu hóa siêu tham số (Hyperparameter Tuning) bằng `RandomizedSearchCV`.
4.  **Đánh giá:** So sánh hiệu suất mô hình qua các chỉ số R², MAE, RMSE.

## 📈 Kết quả nổi bật (Key Findings)
* **Hiệu suất:** Mô hình **XGBoost** đạt kết quả dự báo tốt nhất nhờ khả năng xử lý các mối quan hệ phi tuyến tính và độ trễ thời gian.
* **Tầm quan trọng của tính năng (Feature Importance):**
    * **Seasonality (Tính thời điểm):** Chiếm **58.8%** trọng số tác động.
    * **Khí hậu cực đoan:** Chiếm **27.0%**.
    * **Kinh tế - Xã hội:** Chiếm **5.4%**.
* **Insight:** Xác định rõ vai trò chi phối của bụi mịn PM2.5 và hiện tượng đảo nhiệt đối với áp lực nhập viện của hệ thống y tế.

## 💡 Kết luận (Conclusion)
Dự án khẳng định tiềm năng của việc ứng dụng Big Data trong y tế công cộng. Các mô hình này có thể đóng vai trò như một hệ thống cảnh báo sớm, giúp các chính phủ chủ động hơn trong việc bảo vệ tương lai xanh và sức khỏe cộng đồng.

---

## 📂 Cấu trúc thư mục
* `Air Quality and Health Impact Analysis.ipynb`: File Notebook chi tiết toàn bộ quá trình thực hiện.
* `Raw_data/`: Thư mục chứa bộ dữ liệu.
* `images/`: Các biểu đồ, kết quả trực quan hóa từ dự án.
