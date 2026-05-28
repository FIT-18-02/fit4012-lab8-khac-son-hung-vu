# Lab 8 - Peer review response

## Nhóm được review

- Tên nhóm: Hung Vu Ho Son
- Người review: Hồ Khắc Sơn

## Góp ý nhận được

1. Thiếu file `conftest.py` khiến pytest không tìm được module `secure_transfer_utils` khi chạy từ thư mục `tests/`.
2. File `report-1page.md` còn placeholder ảnh chụp màn hình chưa được điền.
3. Chưa có log minh chứng chạy demo Sender/Receiver trong thư mục `logs/`.

## Phản hồi và chỉnh sửa

| Góp ý | Phản hồi của nhóm | File/commit đã sửa |
|---|---|---|
| Thiếu `conftest.py` | Đã thêm `conftest.py` ở thư mục gốc, dùng `sys.path.insert` để pytest tìm được module từ thư mục con `tests/`. 11/11 test đều pass sau khi sửa. | `conftest.py` |
| Report còn placeholder ảnh | Đã thay placeholder bằng mô tả kết quả chạy demo và đường dẫn log file thực tế. | `report-1page.md` |
| Thiếu log minh chứng | Đã chạy demo local và lưu log vào `logs/sender_success.log` và `logs/receiver_success.log`. | `logs/` |

## Tự đánh giá sau chỉnh sửa

- Chương trình chạy được demo Sender/Receiver: Có
- Có kiểm tra SHA-256: Có
- Có mã hóa DES key bằng RSA-OAEP: Có
- Có test cho packet/tamper: Có
- Có log minh chứng: Có