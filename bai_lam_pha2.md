# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:09**
- **Họ tên:Trần Minh Hiển**
- **Lớp:CNTT3**
- **Link repository Pha2:https://github.com/hanuaa/HN-K26-CNTT3_PromptAI_H02.git**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini): ChatGPT**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt chỗ workshop ra JSON

**KET QUA AI**

```text
[
  {
    "ma_lop": "NAN_GOM",
    "ngay_hoc": "2026-12-13",
    "nguoi_lon": 2,
    "tre_em": 1,
    "ca_hoc": "chieu",
    "ghi_chu": null
  },
  {
    "ma_lop": "BANXOAY",
    "ngay_hoc": "2027-01-10",
    "nguoi_lon": 3,
    "tre_em": 0,
    "ca_hoc": null,
    "ghi_chu": "1 người bị đau cổ tay"
  },
  {
    "ma_lop": "VEGOM",
    "ngay_hoc": null,
    "nguoi_lon": 4,
    "tre_em": 0,
    "ca_hoc": "sang",
    "ghi_chu": "1 bạn đi xe lăn"
  }
]
```

**Link trò chuyện:https://chatgpt.com/share/6b07e344-4488-83ec-acaa-c931c97c5890**

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
**BÁO GIÁ LỚP BANXOAY**

**1. Tiền người lớn**

5 × 550.000 = **2.750.000 đồng**

**2. Tiền trẻ em**

- Trẻ 8 tuổi: 550.000 × 70% = 385.000 đồng
- Trẻ 12 tuổi: 550.000 × 70% = 385.000 đồng
- Bé 4 tuổi: Miễn phí.

Tổng tiền trẻ em = 385.000 × 2 = **770.000 đồng**

**3. Tiền học**

2.750.000 + 770.000 = **3.520.000 đồng**

**4. Giảm giá nhóm**

Nhóm có 5 người lớn, được giảm 5%.

3.520.000 × 5% = 176.000 đồng

Tiền học sau giảm = 3.520.000 − 176.000 = **3.344.000 đồng**

**5. Phí nung và giao sản phẩm**

4 × 80.000 = **320.000 đồng**

**6. Tổng tiền**

3.344.000 + 320.000 = **3.664.000 đồng**

TỔNG THANH TOÁN

# **3.664.000 đồng**

[RESULT]\: 3.664.000 đồng
```

**Link trò chuyện:https://chatgpt.com/share/6b07e387-b7dc-83ec-8783-333b790dab8f**
### b) Kiểm tra kết quả AI

kết quả đúng, đã đáp ứng đủ các yêu cầu 

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "Hỏng sản phẩm khi nung hoặc giao hàng",
  "hong_san_pham": "5 sản phẩm bị nứt vỡ × 150.000 đồng = 750.000 đồng",
  "giao_tre": "Không có thông tin khiếu nại về việc giao trễ. Không áp dụng đền bù.",
  "huong_dan": "Khách hàng hài lòng với thái độ người hướng dẫn. Không áp dụng đền bù. Tổng mức đền bù là 750.000 đồng, vượt ngưỡng 600.000 đồng nên phải được Quản lý xưởng duyệt trước khi gửi khách."
}
```

**Link trò chuyện:https://chatgpt.com/share/6b07e3e0-f3fc-83ec-9412-293526975522**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí                         | Điểm      | Minh chứng                                                                                                                         | Đề xuất sửa                                                                                 |
| -------------------------------- | --------- | ---------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| Chào hỏi và xưng hô              | 2/2       | “Hi chị ơi!” – Cách chào hỏi thân thiện, phù hợp với khách hàng.                                                                   | Không cần sửa.                                                                              |
| Cung cấp thông tin giá           | 1.5/2     | “Lớp vẽ gốm bên em 200k thôi nè” – Có cung cấp giá nhưng chưa nói rõ giá đã bao gồm những dịch vụ nào.                             | “Lớp vẽ gốm bên em có giá 200.000đ/người, bao gồm nguyên vật liệu và dụng cụ thực hành ạ.”  |
| Thông tin chính sách đổi lịch    | 1/2       | “Chị đổi trước 1 ngày thì free nha chị.” – Diễn đạt chưa rõ điều kiện đổi lịch miễn phí, chưa nêu cách thức hoặc giới hạn áp dụng. | “Chị có thể đổi lịch miễn phí nếu thông báo trước ít nhất 24 giờ so với giờ học ạ.”         |
| Thái độ và lời kêu gọi tương tác | 2/2       | “vui lắm luôn. Có gì chị nhắn em nha!” – Giọng điệu gần gũi, tích cực và khuyến khích khách hàng liên hệ.                          | “Lớp học rất vui và phù hợp cho cả người mới bắt đầu. Chị cần tư vấn thêm thì nhắn em nhé!” |
| **Tổng điểm**                    | **6.5/8** | Phản hồi thân thiện, có thông tin giá và chính sách đổi lịch nhưng còn thiếu chi tiết cần thiết.                                   | Nên bổ sung phạm vi giá và điều kiện đổi lịch cụ thể để khách hàng dễ hiểu.                 |
```

**Link trò chuyện:https://chatgpt.com/share/6b07e417-4864-83ec-8557-882de21a6110**
