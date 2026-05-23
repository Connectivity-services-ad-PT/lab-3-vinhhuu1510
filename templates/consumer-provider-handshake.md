# Consumer–Provider Handshake

## Thông tin chung

- Lab: FIT4110 Lab 03
- Ngày: 22/05/2026
- Provider team:
+ IoT Ingestion Team
+ Access Gate Team
+ AI Vision Team
+ Notification Team
+ Analytics Team
- Consumer team:
+ Access Gate Team (consume IoT data)
+ AI Vision Team (consume IoT/Gate data)
+ Notification Team (consume AI/Analytics results)
+ Analytics Team (consume data from IoT, Gate, AI)
+ Mobile/Web App Team
+ API Testing (Postman Consumer)
- Provider service:
+ IoT Ingestion Service
+ Access Gate Service
+ AI Vision Service
+ Notification Service
+ Analytics Service
- Consumer service:
+ AI Vision Service (consumes IoT Ingestion API)
+ Access Gate Service (consumes IoT data API)
+ Notification Service (consumes AI Vision / Analytics API)
+ Analytics Service (consumes IoT / Gate / AI data)
+ Mobile/Web Application (consumes all APIs)

## Contract

* Contract file: contracts/core-business.openapi.yaml
* Mock base URL: http://localhost:4011
* Auth method: Bearer Token
* Endpoint được test: POST /detect

## Smoke test

### Request

POST /detect
Authorization: Bearer lab-token
Content-Type: application/json

```json
{
  "image_url": "http://example.com/test.jpg"
}
```

### Expected response

```json
{
  "result": "ok"
}
```

## Kết quả

* [x] Consumer gọi mock thành công.
* [x] Consumer parse được field cần dùng.
* [x] Consumer hiểu lỗi 4xx/5xx provider trả về.
* [x] Có Newman report hoặc screenshot.

## Ghi chú thay đổi hợp đồng

| Nội dung          | Trước | Sau | Người đồng ý |
| ----------------- | ----- | --- | ------------ |
| Không có thay đổi | -     | -   | -            |

## Xác nhận

* Provider representative: ký tên
* Consumer representative: ký tên




