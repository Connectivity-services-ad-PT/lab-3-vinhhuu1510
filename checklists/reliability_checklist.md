# Reliability Checklist — FIT4110 Lab 03

Điền checklist này trước khi nộp Lab 03.

## 1. Functional tests

- [X] Có test cho endpoint health.
- [X] Có test happy path cho endpoint chính.
- [X] Có kiểm tra status code 2xx.
- [X] Có kiểm tra field quan trọng trong response.
- [X] Có ít nhất 1 test đọc dữ liệu danh sách hoặc chi tiết.

## 2. Auth tests

- [X] Có test thiếu token.
- [X] Có test sai token hoặc token rỗng.
- [X] Endpoint public được khai báo rõ nếu không cần auth.
- [X] Test thể hiện đúng expected status 401/403.

## 3. Negative tests

- [X] Có test thiếu field bắt buộc.
- [X] Có test sai kiểu dữ liệu.
- [X] Có test sai enum hoặc giá trị ngoài miền.
- [X] Lỗi trả về theo cùng một error model.

## 4. Boundary tests

- [X] Có test min/max hoặc dữ liệu sát ngưỡng.
- [X] Có test limit/pagination nếu endpoint có danh sách.
- [X] Có test payload lớn hoặc metadata thiếu.
- [X] Có ghi chú kỳ vọng xử lý dữ liệu biên.

## 5. Reliability tests cơ bản

- [X] Có kiểm tra response time.
- [X] Có mô tả timeout mong muốn.
- [X] Có test hoặc ghi chú retry/idempotency nếu phù hợp.
- [X] Có consumer-side smoke test với ít nhất 1 mock của nhóm khác.

## 6. Evidence

- [X] Collection export JSON.
- [X] Environment mock export JSON.
- [X] Environment local export JSON.
- [X] Newman report XML/HTML.
- [X] Test-case matrix đã điền.
- [X] Biên bản handshake đã điền.
