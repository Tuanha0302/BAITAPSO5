# BAITAPSO5
## Tạo 1 database mới mang tên SoLienLacDienTu 
![image](https://github.com/user-attachments/assets/c6771368-e704-4680-a1f8-77a233d12273)

## Tạo 1 bảng mang tên HocSinh 
+ có mã học sinh là khóa chính và 4 cột khác là: tên học sinh, lớp, ngày sinh, giới tính
+ không có điều kiện ở cột nào
+ có khóa ngoại là mã học sinh
![image](https://github.com/user-attachments/assets/c1c91282-7fa2-4ea8-ab4b-b1187500a302)

## Tạo 1 bảng mang tên MonHoc
+ có mã môn là khóa chính và 1 cột khác là: tên môn
+ không có điều kiện ở cột nào
+ có khóa ngoại là mã môn
![image](https://github.com/user-attachments/assets/09366b89-b4b2-4008-9f7c-57faeea1f672)

## Tạo 1 bảng mang tên DiemSo
+ có mã học sinh, mã môn là khóa chính và có 4 cột khác là: điểm hệ số 1, điểm hệ số 2, điểm thi, điểm trung bình
+ có 3 điều kiện là:
  + điểm hệ số 1: ([DiemHeSo1]>=(0) AND [DiemHeSo1]<=(10))
  + điểm hệ số 2: ([DiemHeSo2]>=(0) AND [DiemHeSo2]<=(10))
  + điểm thi: ([DiemThi]>=(0) AND [DiemThi]<=(10))
  ![image](https://github.com/user-attachments/assets/065181bc-8377-4d7b-b49d-7c0f95dcf05c)
+ điểm hệ số 1 là 2 loại điểm: điểm kiểm tra miệng và điểm kiểm tra 15 phút
+ điểm hệ số 2 là điểm kiểm tra 1 tiết
+ điểm hệ số 3 là điểm thi
  
=> để giúp tính điểm trung bình với công thức: ĐTB= (HS1+HS2×2+Thi×3)/6

+ có khóa ngoại là mã học sinh, mã môn
![image](https://github.com/user-attachments/assets/f3d41c3f-e70e-4a71-9d08-30fc3f172b3f)

## Tạo 1 bảng mang tên PhanHoi 
+ có mã phản hồi là khóa chính và có 3 cột khác là: mã học sinh, nội dung, ngày gửi
+ không có điều kiện ở cột nào
+ có khóa ngoại là mã phản hồi
![image](https://github.com/user-attachments/assets/ca3ff6a7-cc14-42d4-8f9a-7a64c5b55335)

## Tạo 1 bảng mang tên cảnh báo
+ ở bảng này ta không tạo khóa chinh, khóa ngoại, điều kiện
+ vì ở bảng này ta sẽ dùng để ghi lại các cảnh báo tự động từ trigger và vì có trigger tính toán sẵn nên không cần ràng buộc điều kiện nào
![image](https://github.com/user-attachments/assets/1b625685-6dc8-49ac-93cd-bd873cbd3ec4)

## Sơ đồ dữ liệu SoLienLacDienTu
![image](https://github.com/user-attachments/assets/0c2d86d0-caa1-44e5-ab1a-7dbe55a66af8)

## Dùng lệnh để nhập dữ liệu cho bảng HocSinh
![image](https://github.com/user-attachments/assets/22ecee9b-a291-4560-91b9-cd3eddc76cd6)

+ ta cũng sẽ nhập bảng MonHoc bằng cách như trên
  
![image](https://github.com/user-attachments/assets/4c095e2d-316c-411b-af4f-dde3a0df1d16)

## Trigger tự động tính điẻm trung bình và cảnh báo điểm thấp 
+ Trigger tự động tính điểm trung bình
![Ảnh chụp màn hình 2025-04-20 230849](https://github.com/user-attachments/assets/4a90199d-33ac-47f9-88d5-04d3f048dbd7)

+ Trigger cảnh báo điểm thấp
![Ảnh chụp màn hình 2025-04-20 232123](https://github.com/user-attachments/assets/9c44ad0e-88cb-4eb3-9252-cf7189c31097)

## Kiểm tra kết quả 
![image](https://github.com/user-attachments/assets/13febed4-465c-4c5d-ad54-72f4d00280ce)








