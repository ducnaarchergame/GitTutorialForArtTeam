# I. Quy định về quản lý máy môi trường
- Mỗi máy môi trường sẽ do 1 người quản lý và chịu trách nhiệm . Sẽ có username/password và chỉ có người quản lý biết password. 
- Khi có người có nhu cầu sử dụng tạm thời máy môi trường, sẽ phải có sự đồng ý từ người quản lý máy. Khi đồng ý, người quản lý máy có trách nhiệm nhập password và đảm bảo rằng tất cả công việc ở máy này đã được push lên server. Trong thời gian này, người quản lý máy không sử dụng máy đến khi nhận hoàn trả từ người đang tạm thời sử dụng. 
- Khi hoàn thành xong công việc, người sử dụng máy cần commit push lên server và hoàn trả cho người quản lý máy đó. 
  

# II. Quy định làm việc

## 1. Trước khi bắt đầu công việc
- Cần pull code mới nhất từ server về
- Đảm bảo trên máy local đang không có thay đổi gì (Nothing to commit)

## 2. Sau khi hoàn tất công việc:

### Unity
- Save (Ctrl+S) trước khi commit push / pull

### Git
#### Step 2.1: Lựa chọn những thay đổi của mình để add vào stage

#### Step 2.2: Commit ở local

#### Step 2.4: Push to server
- Pull lại code mới nhất
- Push lên server
 
## 3. Recommendations
- Nên commit thường xuyên để tránh việc mất mát (recommend ít nhất nửa ngày 1 lần)
- Team Art sẽ làm việc trên 1 nhánh riêng là nhánh **teamart**
