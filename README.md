# Project_CustomerReview_SentimentAnalysis
Đồ án cuối kỳ môn Xử lý ngôn ngữ tự nhiên (UEH)

# Mô tả bộ dữ liệu
Bộ dữ liệu Women's E-Commerce Clothing Reviews chứa thông tin đánh giá của khách hàng về sản phẩm, được sử dụng cho các bài toán NLP (Sentiment Analysis), bao gồm 10 thuộc tính và 23.486 dòng dữ liệu.
Bộ dữ liệu có thể tìm thấy ở [Kaggle](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews)

- **Clothing ID**: Mã sản phẩm
- **Age**: Tuổi của khách hàng
- **Title**: Tiêu đề bài review
- **Review Text**: Nội dung bài review
- **Rating**: Đánh giá (từ 1-5 sao)
- **Recommended IND**: Biến nhị phân cho biết sản phẩm có được recommend hay không (1 = recommended, 0 = unrecommended)
- **Positive Feedback Count**: Số lượng khách hàng nhận thấy đánh giá này là tích cực
- **Division Name**: Tên phân loại sản phẩm
- **Department Name**: Tên nhóm sản phẩm
- **Class Name**: Tên lớp sản phẩm

# Tổng quan dự án
1. **EDA (Exploratory Data Analysis):** Thăm dò dò bộ dữ liệu trước khi tiến hành tiền xử lý và vẽ biểu đồ tương quan giữa các biến.
2. **Tiền xử lý dữ liệu:**: Xử lý missing values, chỉnh dạng dữ liệu để chuẩn bị cho quá trình Text Mining
3. **Text Mining:** Xử lý, trích xuất và khai thác thông tin trong dữ liệu văn bản (đánh giá của khách hàng)
4. **WordCloud:**: Vẽ biểu đồ Word Cloud thể hiện các từ có tần suất xuất hiện cao trong văn bản, phân theo review tích cực, review tiêu cực, và review tổng thể.
5. **Sentiment Analyst:** Áp dụng 2 mô hình phân lớp Naive Bayes và Logistic Regression sử dụng thư viện NLTK để thu thập phản hồi của khách hàng về sản phẩm (tích cực và tiêu cực). Đánh giá mô hình huấn luyện.
