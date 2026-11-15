# Repository mẫu — Bộ bài HSG Tin học (MC.Thọ)

Mẫu này có thể đưa nguyên nội dung lên một repository **public** mới tại `https://github.com/maicuongtho/<ten-repository>`.

```text
topics.json                                  # tên chuyên đề
  topics/nhap-xuat/TONG/statement.md        # đề bài Markdown UTF-8
  topics/nhap-xuat/TONG/config.json         # cấu hình chấm
  topics/nhap-xuat/TONG/tests/001.in        # dữ liệu
  topics/nhap-xuat/TONG/tests/001.out       # đáp án
  topics/mang/SUM_ARRAY/statement.md
  topics/mang/SUM_ARRAY/config.json
  topics/mang/SUM_ARRAY/tests/001.in
  topics/mang/SUM_ARRAY/tests/001.out
```

Các trường `topics.json`: danh sách `topics`: `{ "id": "so-hoc", "title": "Số học và tổ hợp" }`.

Quy tắc:

- Mã chuyên đề là chữ thường không dấu, số, `_` và `-`; bắt đầu bằng chữ, ví dụ `quy-hoach-dong`.
- Mã bài là chữ IN HOA, số và `_`; bắt đầu bằng chữ, ví dụ `TONG`, `UCLN`, `DAY_SO`.
- Đề bài **bắt buộc** `statement.md`, viết UTF-8, tiêu đề `# ...`.
- `config.json` tùy chọn: `io_mode` là `file` hoặc `stdio`; `time_limit` (giây); `compare` là `tokens` hoặc `exact`; thêm `input_file`/`output_file` với chế độ `file`.
- Mỗi test dùng cặp tên trùng nhau `001.in` và `001.out`. Cho phép nhiều test: `002.in`, `002.out`...
- Có thể đặt ảnh trong `topics/<chuyen-de>/<MA_BAI>/assets/hinh.png` và dẫn bằng Markdown `![Hình](assets/hinh.png)`. Hỗ trợ PNG/JPG/GIF/WebP.
- Không đưa mã nguồn lời giải mẫu vào repo của học sinh. Web App **không tải tệp `.py` từ GitHub**.
- Có thể chia nhiều repository theo lớp, chủ đề hoặc bộ đề; một repo chứa nhiều chuyên đề/bài. Khi cập nhật repo, học sinh tự bấm Đồng bộ để tải thay đổi.

Ứng dụng hiện chỉ tải repo công khai thuộc tài khoản `maicuongtho`; không dùng token hoặc truy cập repo riêng tư. Trong trường hợp Github API rate limit, đợi hoặc nhập URL lại sau.
