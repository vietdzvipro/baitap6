# baitap6
Bài tập 6: Hệ quản trị CSDL
Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
Cho file sv_tnut.sql (1.6MB)
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

DEADLINE: 23H59:59 NGÀY 25/4/2025

Ghi chú: Giải thích tại sao lại có SQL như vậy.

## CÁC BƯỚC ĐỂ IMPORT DỮ LIỆU TRONG sv_tnut.sql vào sql server

![image](https://github.com/user-attachments/assets/d5ee6b38-7a66-42e8-a4c2-1173841a3e34)

- Sau đó vào file chọn open và mở file sv_tnut.sql của thầy

![image](https://github.com/user-attachments/assets/f7b474ce-1728-4922-bb2a-0ee3faec0796)

- Sau khi mở file sql thì execute(f5) để cập nhật dữ liệu vào database

![image](https://github.com/user-attachments/assets/1cb05897-8333-4ad7-8df3-dc595e17c90d)

- Đây là hình ảnh sau khi import thành công

![image](https://github.com/user-attachments/assets/d121a422-4fe1-42b7-8627-639ecd04bef0)

## TRUY VẤN DỮ LIỆU CỦA SV ĐANG LÀM BÀI TẬP NÀY

![image](https://github.com/user-attachments/assets/7dd58e38-ef23-409c-8339-01d170c75c06)

## TÌM RA NHỮNG SINH VIÊN TRÙNG NGÀY THÁNG NĂM SINH

![image](https://github.com/user-attachments/assets/dd807132-dc3b-4ea9-9353-383b096729e8)

## TÌM RA NHỮNG SINH VIÊN TRÙNG NGÀY VỚI THÁNG SINH

![image](https://github.com/user-attachments/assets/5f1d3e29-2fe8-4894-a4ab-b215a1a49649)

## TÌM RA NHỮNG SINH VIÊN TRÙNG THÁNG VỚI NĂM SINH

![image](https://github.com/user-attachments/assets/fe747d33-0818-413f-9920-6d53e05fcba2)

## TÌM RA NHỮNG SINH VIÊN TRÙNG TÊN

![image](https://github.com/user-attachments/assets/1190cd1e-a2f4-438a-8314-4b69f6799bd9)

## TÌM RA NHỮNG SINH VIÊN TRÙNG HỌ VỚI TÊN ĐỆM

![image](https://github.com/user-attachments/assets/c89c92d2-4117-4036-a200-6d3fadb0a0d6)

## TÌM RA NHỮNG SINH VIÊN CÓ SDT SAI KHÁC CHỈ MỘT SỐ 

- Dùng lệnh để kiểm tra những sinh viên có sdt sai khác 1 số kh có sinh viên nào nên khi chạy lệnh sẽ kh hiện ra gì như dưới đây

![image](https://github.com/user-attachments/assets/cbfc886b-0a49-4134-8077-d7996603d1ff)

- Vì vậy chúng ta sẽ thêm số ký tự sai so với số của em để kiểm tra lần nữa cho chắc xem có sdt nào sai chỉ 1 số không

![image](https://github.com/user-attachments/assets/9f11a3ef-2779-49d6-bc70-c77da460872e)

##  BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH

- Để xem được 9000 rows thì ta chỉ cần dùng select top (10000) là được

![image](https://github.com/user-attachments/assets/e8a000f3-1c03-47b3-8745-bfa3ddee0884)

## Giải thích:
- SELECT TOP (10000)
- SELECT: Đây là lệnh SQL dùng để lấy dữ liệu từ bảng.
- TOP (10000): Lấy tối đa 10.000 dòng kết quả. Điều này giúp bạn giới hạn số lượng dòng dữ liệu, tránh việc truy vấn quá nhiều dữ liệu mà có thể gây ra lỗi hoặc quá tải trong môi trường SQL. Nếu bảng có ít dữ liệu hơn, hệ thống vẫn sẽ trả về toàn bộ dữ liệu có sẵn.
- Lý do sử dụng TOP: Trong trường hợp bạn có bảng có quá nhiều dòng (hơn 9000 dòng như bạn đã nói), dùng TOP (10000) sẽ giúp truy vấn không bị gián đoạn.

## Tổng quan về kết quả:
- Truy vấn này sẽ trả về danh sách sinh viên thuộc lớp có tên chứa "KMT", được sắp xếp theo lớp từ bé đến lớn và trong mỗi lớp, sinh viên sẽ được sắp xếp theo tên từ A đến Z.
- Lý do sử dụng COLLATE Vietnamese_CI_AS: Đây là cách để sắp xếp dữ liệu theo quy tắc tiếng Việt, phân biệt dấu (tức là "a" và "á" được xem là khác nhau), nhưng không phân biệt chữ hoa và chữ thường.

## LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV

- Dưới đây là code và các sinh viên nữ trong ngành kmt:

![image](https://github.com/user-attachments/assets/e922f3f2-4149-4e9c-b1be-115805ce556d)

## Làm sao biết sinh viên là "nữ"?
- Bảng SV không có cột gioitinh (giới tính)? Vậy phải suy đoán từ tên.
## Ta có thể giả định rằng:
- Các sinh viên có tên như: “Lan”, “Hương”, “Hạnh”, “Mai”, “Trang”, “Ngọc”,… là nữ.
- Điều này không hoàn toàn chính xác, nhưng là cách tạm chấp nhận được nếu không có cột giới tính.
- Do đó, ta có thể lọc tên có chứa các chuỗi “Lan”, “Hương”, v.v. bằng LIKE.
