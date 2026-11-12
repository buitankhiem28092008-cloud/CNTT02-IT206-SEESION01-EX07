# Bài 7: Thiết kế Quy trình Che mờ (Data Masking) Khách VIP
## Phần A: Bảng Che mờ (Masking Table)
- Phạm Minh C $\rightarrow$ [TEN_KHACH_HANG] (Họ tên)
- 0988.111.222 $\rightarrow$ [SO_DIEN_THOAI] (SĐT)
- minhc@gmail.com $\rightarrow$ [EMAIL] (Email)  
- Căn hộ 502 Chung cư Sunrise, Q7 $\rightarrow$ [DIA_CHI] (Địa chỉ)
## Phần B: Masked Input
"Tôi là [TEN_KHACH_HANG] (SĐT: [SO_DIEN_THOAI], Email: [EMAIL], ở [DIA_CHI]). Ngày 20/09 tôi mua 2kg thịt bò Wagyu giá 4.500.000 VNĐ tại MartX District 7 nhưng bị giao chậm 3 tiếng làm hỏng tiệc gia đình. Tôi yêu cầu bồi thường 100%!"
## Phần C: Prompt gửi AI 
"Đóng vai Trưởng bộ phận CSKH MartX. Viết email xin lỗi lịch sự, nhận lỗi giao chậm 3 tiếng đơn hàng 2kg thịt bò Wagyu (4.500.000 VNĐ) ngày 20/09, đồng ý bồi thường 100%. Giữ nguyên các nhãn [TEN_KHACH_HANG], [SO_DIEN_THOAI], [EMAIL], [DIA_CHI]. Nội dung khiếu nại: [Dán Phần B]"
## Phần D: Văn bản De-mask
- [x] kính gửi Anh/Chị Phạm Minh C, MartX chân thành xin lỗi vì sự cố giao chậm 3 tiếng đơn hàng 2kg thịt bò Wagyu (4.500.000 VNĐ) ngày 20/09 làm hỏng tiệc gia đình Anh/Chị. Là khách hàng VIP, chúng tôi đồng ý hoàn tiền 100%.

- [x] Nhân viên sẽ liên hệ số 0988.111.222 và gửi chi tiết qua email minhc@gmail.com để giao bồi thường tận nơi tại Căn hộ 502 Chung cư Sunrise, Q7.   Trân trọng,CSKH MartX 