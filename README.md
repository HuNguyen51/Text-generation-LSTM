# Sinh từ sử dụng model RNN (LSTM) với dữ liệu được lấy từ github
(https://github.com/hoanganhpham1006/Vietnamese_Language_Model/blob/master/Train_Full.zip)

- Trong bài này mình sẽ tạo ra 3 file code chính
    - preprocess.ipynb -> dùng để tiền xử lý dữ liệu như đọc data, làm sạch rồi lưu lại thành file train.txt cho quá trình tiếp theo
    - LSTM-Text_Generation-Model.ipynb -> lấy dữ liệu từ train.txt, tự định nghĩa tokenizer từ dữ liệu đầu vào, dựa vào cấu trúc dữ liệu ra trích xuất ra các đặc trưng và nhãn rồi tạo model và huấn luyện model
    - implement-Text_Generation.ipynb -> dùng tokenizer và model đã được huấn luyện từ trước và định nghĩa các hàm sinh văn bản
- Model sẽ nhận đầu vào với shape là (, 50), và trả về đầu ra là (,vocab_size)
- Đầu ra giống với categorical ra sử dụng hàm kích hoạt là softmax để lấy phân phối xác xuất cao nhất cho 1 từ bằng argmax của numpy
- Hiện nay ngoài RNN ra thì còn rất nhiều các model khác dùng để sinh từ và phải kể đến hiện đại nhất hiện nay là công nghệ GPT
Note: thứ tự chạy các file: preprocess.ipynb -> LSTM-Text_Generation-Model.ipynb -> implement-Text_Generation.ipynb