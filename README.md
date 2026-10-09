# BÁO CÁO BÀI TẬP: CHUẨN HÓA ACCEPTANCE CRITERIA THEO GIVEN-WHEN-THEN

**Tên bài tập:** [VẬN DỤNG CƠ BẢN] CHUẨN HÓA ACCEPTANCE CRITERIA THEO GIVEN-WHEN-THEN

**Vai trò:** Vy (Developer phụ trách kiểm thử)

### Phần 1 - Phân tích

Dưới đây là bảng phân tích Acceptance Criteria (AC) cho chức năng "Áp mã khuyến mãi" dựa trên các quy tắc nghiệp vụ và bối cảnh đã cho.

| AC  | Đúng/Sai | Quy tắc bị vi phạm                                      | Hậu quả khi kiểm thử                                                                  |
| :-- | :------- | :------------------------------------------------------ | :------------------------------------------------------------------------------------ |
| AC1 | Đúng     | (Không vi phạm)                                         | AC đúng cấu trúc Given-When-Then, mỗi AC một kịch bản, kết quả cụ thể, dễ dàng kiểm thử. |
| AC2 | Sai      | - When: đúng một hành động của người dùng               | - Tester không biết chính xác hành động nào cần thực hiện để kiểm thử.               |
|     |          | - Then: kết quả cụ thể                                  | - Không biết kết quả mong đợi là gì để xác nhận "phù hợp".                          |
| AC3 | Sai      | - Given: trạng thái có sẵn trước khi hành động xảy ra   | - Tester không biết trạng thái ban đầu để kiểm thử.                                 |
|     |          | - When: đúng một hành động của người dùng               | - Hành động của người dùng bị đảo ngược thành điều kiện.                             |
| AC4 | Đúng     | (Không vi phạm)                                         | AC đúng cấu trúc Given-When-Then, mỗi AC một kịch bản, kết quả cụ thể, dễ dàng kiểm thử. |

### Phần 2 - Sửa lỗi

Viết lại các AC sai để đảm bảo tuân thủ cấu trúc Given-When-Then và các quy tắc nghiệp vụ.

**AC2 (Sửa): Mã khuyến mãi hết hạn**
*   **Given** khách đang ở màn hình đặt xe với cước chuyến,
*   **Given** mã "GO20" đã hết hạn,
*   **When** khách áp mã "GO20",
*   **Then** hệ thống hiển thị thông báo "Mã khuyến mãi đã hết hạn".

**AC3 (Sửa): Mã khuyến mãi không tồn tại**
*   **Given** khách đang ở màn hình đặt xe với cước chuyến,
*   **Given** mã "ABC123" không tồn tại trong hệ thống,
*   **When** khách áp mã "ABC123",
*   **Then** hệ thống hiển thị thông báo "Mã khuyến mãi không hợp lệ".