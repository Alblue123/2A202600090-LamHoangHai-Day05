# 2A 202600090 - Lâm Hoàng Hải - AI Moni

## P1

* **Sản phẩm hứa hẹn có các chức năng:** Theo dõi chi tiêu, lập kế hoạch ngân sách, tư vấn tiết kiệm, giải đáp thắc mắc về Momo, gợi ý chi tiêu.
* **AI:**
  * Đề xuất những câu hỏi liên quan.
  * Khi đang trả lời thì hiện dòng "thinking..." ≈ "Chờ Moni xíu nha...", reasoning.
  * Có nút đánh giá, đề xuất câu hỏi dựa trên nội dung chat.

---

## P2

**CH1: Khi AI đúng**

* **Câu hỏi:** "Cho tôi báo cáo tài chính năm 2025"
* **Trả lời:** AI trả lời tổng số chi tiêu, tổng số giao dịch, trung bình.
* Tuy nhiên người dùng chỉ biết mình đúng bằng cách kiểm tra lại mục chi tiêu, không cung cấp dẫn chứng thuyết phục hơn.

**CH2: Khi AI không chắc**

* **Câu hỏi_1:** "Cho tôi báo cáo chi tiết từng hạng mục"
* **Trả lời:** AI cung cấp lại chi tiêu tổng, xin lỗi không cung cấp được danh sách chi tiết, yêu cầu trả lời từng hạng mục.
* **Câu hỏi_2:** "Cho tôi đi du lịch"
* **Trả lời:** AI đề xuất các địa điểm du lịch nổi tiếng thay vì chỉ định một địa điểm cụ thể

**CH3: Khi AI sai**

* Người dùng có biết nếu AI sai không?
* **Giả định TH:** "Bảo AI tính chi tiêu ăn uống sai rồi"
* **Các bước:** AI sẽ khẳng định mình không sai, và yêu cầu người dùng tự kiểm tra lại.

**CH4: Khi User mất tin**

* AI không có fallback liên hệ đến tư vấn viên
* Tuy nhiên người dùng có thể dùng Mo Mo mà không cần đến AI

**Đánh giá chung:**

* Path yếu nhất là path 3, AI luôn khẳng định mình đúng.
* Path xử lý tốt nhất là "không chắc", vì nó có thể tự nhận định mình không hỗ trợ, và không đưa thông tin sai.
* Về thực tế, AI Moni vẫn trả lời được những tác vụ đề ra, tuy nhiên thiếu chức năng cho người dùng chứng minh lại, phải làm manual.

---

## P3

| AS-IS                                                   | TO-BE                                                                                        |
| :------------------------------------------------------ | :------------------------------------------------------------------------------------------- |
| **Người dùng kiểm tra lại và thấy AI sai** | **Người dùng nói AI sai**                                                          |
| -> Moni khẳng định không sai                        | -> AI đưa ra link đến dẫn chứng chứng minh rằng mình đúng thay vì khẳng định. |
| -> Yêu cầu người dùng xem lại                     | -> Nếu sai thật thì cho người dùng sửa.                                               |
| -> Người dùng bảo mình không sai -> X (Bế tắc)  |                                                                                              |
