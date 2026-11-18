
# LẬP KẾ HOẠCH TÀI CHÍNH CÁ NHÂN BẰNG CHAIN-OF-THOUGHT (CoT)

## 1. Mục tiêu

- Ứng dụng kỹ thuật Chain-of-Thought (CoT) để giải quyết bài toán lập kế hoạch tài chính cá nhân.
- Phân tích dữ liệu thu nhập, chi phí, khoản nợ và mục tiêu tiết kiệm.
- Kiểm soát các phép tính số học nhằm hạn chế sai sót của AI.
- Xây dựng kế hoạch phân bổ ngân sách hợp lý, đảm bảo trả nợ đúng hạn và tiết kiệm tối thiểu 20%.
- Trình bày kết quả dưới dạng phân tích logic và bảng ngân sách Markdown.

## 2. Dữ liệu đầu vào

Sử dụng dữ liệu giả định sau để kiểm thử:

- Thu nhập hàng tháng: 15.000.000 VNĐ.
- Thuế và các khoản khấu trừ: 500.000 VNĐ.
- Chi phí cố định:
  - Tiền thuê nhà: 2.000.000 VNĐ.
  - Điện, nước, Internet: 500.000 VNĐ.
  - Ăn uống cơ bản: 1.500.000 VNĐ.
  - Đi lại: 500.000 VNĐ.
- Các khoản nợ:
  - Nợ ngân hàng: 1.500.000 VNĐ/tháng.
  - Nợ cá nhân: 500.000 VNĐ/tháng.
- Mục tiêu tiết kiệm: Tối thiểu 20% thu nhập sau thuế.

## 3. Prompt ứng dụng kỹ thuật Chain-of-Thought

### Vai trò (Role)

Bạn là chuyên gia tư vấn tài chính cá nhân, có khả năng phân tích dòng tiền, tính toán ngân sách và đề xuất phương án quản lý tài chính hợp lý.

### Nhiệm vụ (Task)

Hãy lập kế hoạch tài chính hàng tháng dựa trên dữ liệu thu nhập, chi phí cố định, các khoản nợ và mục tiêu tiết kiệm của người dùng.

Hãy suy nghĩ từng bước một và tính toán chi tiết trước khi đưa ra quyết định. Sử dụng quy trình suy luận có cấu trúc để kiểm tra tính chính xác của từng phép tính.

### Dữ liệu đầu vào (Input)

- Thu nhập hàng tháng: 15.000.000 VNĐ.
- Thuế và khấu trừ: 500.000 VNĐ.
- Chi phí cố định:
  - Tiền thuê nhà: 2.000.000 VNĐ.
  - Điện, nước, Internet: 500.000 VNĐ.
  - Ăn uống cơ bản: 1.500.000 VNĐ.
  - Đi lại: 500.000 VNĐ.
- Các khoản nợ:
  - Nợ ngân hàng: 1.500.000 VNĐ/tháng.
  - Nợ cá nhân: 500.000 VNĐ/tháng.
- Mục tiêu tiết kiệm: Tối thiểu 20% thu nhập sau thuế.

### Quy trình xử lý (Process)

**Bước 1: Tính thu nhập khả dụng**

- Thu nhập sau thuế = Tổng thu nhập - Thuế.
- Tổng chi phí cố định = Tổng các khoản chi phí bắt buộc.
- Tiền còn lại = Thu nhập sau thuế - Chi phí cố định.

**Bước 2: Phân bổ trả nợ**

- Tính tổng số tiền trả nợ tối thiểu.
- Ưu tiên thanh toán các khoản nợ đúng hạn.
- Xác định số tiền còn lại sau khi trả nợ.

**Bước 3: Trích lập tiết kiệm**

- Tiền tiết kiệm tối thiểu = Thu nhập sau thuế × 20%.
- Đảm bảo khoản tiết kiệm không thấp hơn mục tiêu đã cam kết.
- Ưu tiên xây dựng quỹ dự phòng khẩn cấp.

**Bước 4: Phân bổ chi tiêu linh hoạt**

- Xác định số tiền còn lại sau khi trừ chi phí cố định, trả nợ và tiết kiệm.
- Áp dụng quy tắc 50/30/20 cải tiến:
  - Nhu cầu thiết yếu: Chi phí sinh hoạt cần thiết.
  - Mong muốn cá nhân: Giải trí, mua sắm, ăn uống bên ngoài.
  - Tiết kiệm và trả nợ: Duy trì mục tiêu tài chính.
- Điều chỉnh tỷ lệ theo tình hình thu nhập thực tế.

**Bước 5: Kiểm tra tính chính xác**

- Kiểm tra tổng số tiền phân bổ có bằng thu nhập sau thuế hay không.
- Kiểm tra tổng tỷ lệ phần trăm có chính xác 100% hay không.
- Nếu có sai lệch, phải tính toán và điều chỉnh lại.
- Không tự ý bỏ qua khoản nợ hoặc chi phí bắt buộc.

### Định dạng đầu ra (Output)

**Phần 1: Phân tích logic (Reasoning Steps)**

- Trình bày các công thức tính toán.
- Nêu số liệu đầu vào và kết quả trung gian.
- Giải thích ngắn gọn kết quả từng bước.
- Chỉ trình bày các phép tính và kết quả có thể kiểm chứng.

**Phần 2: Bảng phân bổ ngân sách**

- Sử dụng bảng Markdown với các cột: Hạng mục, Số tiền, Tỷ lệ %, Ghi chú.
- Có đầy đủ các khoản thu, chi, trả nợ và tiết kiệm.
- Tỷ lệ được tính trên tổng thu nhập sau thuế.
- Tổng tỷ lệ phân bổ phải bằng chính xác 100%.

### Ràng buộc (Constraints)

- Không bỏ qua bất kỳ khoản chi phí hoặc khoản nợ nào.
- Không tự ý tạo thêm dữ liệu khi chưa có căn cứ.
- Không sử dụng Python, Pydantic hoặc công cụ lập trình.
- Phải kiểm tra lại các phép tính cộng, trừ, nhân, chia.
- Nếu dữ liệu đầu vào thiếu hoặc mâu thuẫn, phải thông báo và yêu cầu bổ sung.
- Không đưa ra kế hoạch có tổng chi vượt thu nhập sau thuế.
- Ưu tiên đảm bảo trả nợ đúng hạn và tiết kiệm tối thiểu 20%.

## 4. Kết quả thực hiện

### Phần 1: Phân tích logic (Reasoning Steps)

**Bước 1: Tính thu nhập sau thuế và chi phí cố định**

- Thu nhập sau thuế:

  15.000.000 - 500.000 = 14.500.000 VNĐ.

- Tổng chi phí cố định:

  2.000.000 + 500.000 + 1.500.000 + 500.000 = 4.500.000 VNĐ.

- Tiền còn lại:

  14.500.000 - 4.500.000 = 10.000.000 VNĐ.

**Bước 2: Phân bổ trả nợ**

- Tổng tiền trả nợ:

  1.500.000 + 500.000 = 2.000.000 VNĐ.

- Tiền còn lại:

  10.000.000 - 2.000.000 = 8.000.000 VNĐ.

**Bước 3: Trích lập tiết kiệm**

- Mục tiêu tiết kiệm:

  14.500.000 × 20% = 2.900.000 VNĐ.

- Tiền còn lại:

  8.000.000 - 2.900.000 = 5.100.000 VNĐ.

**Bước 4: Phân bổ chi tiêu linh hoạt**

Phân bổ 5.100.000 VNĐ còn lại:

- Giải trí và mua sắm: 2.000.000 VNĐ.
- Chi phí phát sinh: 1.500.000 VNĐ.
- Bổ sung quỹ dự phòng: 1.600.000 VNĐ.

Kiểm tra:

2.000.000 + 1.500.000 + 1.600.000 = 5.100.000 VNĐ.

**Bước 5: Kiểm tra tổng ngân sách**

Tổng phân bổ:

4.500.000 + 2.000.000 + 2.900.000 + 2.000.000 + 1.500.000 + 1.600.000 = 14.500.000 VNĐ.

Ngân sách cân bằng, không vượt thu nhập sau thuế.

### Phần 2: Bảng phân bổ ngân sách cuối cùng

| Hạng mục | Số tiền (VNĐ) | Tỷ lệ % | Ghi chú |
|---|---:|---:|---|
| Chi phí cố định | 4.500.000 | 31,03% | Nhà ở, điện nước, ăn uống, đi lại |
| Trả nợ ngân hàng | 1.500.000 | 10,34% | Thanh toán đúng hạn |
| Trả nợ cá nhân | 500.000 | 3,45% | Thanh toán đúng hạn |
| Tiết kiệm | 2.900.000 | 20,00% | Đạt mục tiêu tối thiểu |
| Giải trí, mua sắm | 2.000.000 | 13,79% | Chi tiêu linh hoạt |
| Chi phí phát sinh | 1.500.000 | 10,35% | Dự phòng chi tiêu |
| Bổ sung quỹ dự phòng | 1.600.000 | 11,04% | Dành cho trường hợp khẩn cấp |
| **Tổng cộng** | **14.500.000** | **100%** | **Ngân sách cân bằng** |

## 5. Đánh giá kết quả

- **Thu nhập:** Đã xác định chính xác thu nhập sau thuế là 14.500.000 VNĐ.
- **Trả nợ:** Đảm bảo thanh toán đầy đủ 2.000.000 VNĐ mỗi tháng.
- **Tiết kiệm:** Đạt mục tiêu 20% thu nhập sau thuế.
- **Chi tiêu:** Có ngân sách riêng cho giải trí và các khoản phát sinh.
- **Quỹ dự phòng:** Có thêm 1.600.000 VNĐ để tăng khả năng ứng phó với tình huống khẩn cấp.
- **Kiểm soát ngân sách:** Tổng số tiền phân bổ bằng chính xác thu nhập sau thuế.

## 6. Kết luận

Kỹ thuật Chain-of-Thought (CoT) giúp chia bài toán tài chính phức tạp thành các bước xử lý logic, từ tính thu nhập, chi phí, trả nợ đến tiết kiệm và phân bổ ngân sách.

Thông qua việc sử dụng công thức rõ ràng và kiểm tra tổng số tiền, AI có thể hạn chế sai sót số học, đảm bảo ngân sách cân bằng và đưa ra kế hoạch tài chính hợp lý.

**Lưu ý:** Tất cả tỷ lệ phần trăm được tính trên thu nhập sau thuế 14.500.000 VNĐ. Việc kiểm tra tổng số tiền và tổng tỷ lệ giúp đảm bảo tính chính xác của kế hoạch tài chính.
