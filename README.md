# Bài tập về bài toán Time-series trên bộ dữ liệu thời tiết được lấy từ kaggle với mục tiêu là dự đoán giá trị thời tiết của những ngày tiếp theo
- Trong bài này mình sử dụng model mạng thần kinh với các layers LSTM và Dropout để hạn chế overfitting
- Ngoài ra còn sử dụng thêm Bidirectional LSTM
- Về lý thuyết thì LSTM mô hình thích hợp để sử dụng cho một chuỗi giá trị có thứ tự, nhưng hạn chế của nó là đối với dữ liệu quá dài thì phần sau nó không thể học tốt được
- Bidirectional LSTM có thể giải quyết phần nào hạn chế này vì cơ chế của nó là học thứ từ từ đầu đến cuối và ngược lại từ cuối trở lên đầu nhưng những dữ liệu quá dài thì phần giữa sẽ gặp hạn chế (vì nó quá xa so với điểm xuất phát)
- Ngày nay các mô hình sử dụng dữ liệu dạng chuỗi lớn tốt có thể kể đến như transformer và mình sẽ có một bài về lĩnh vực này sau

 
