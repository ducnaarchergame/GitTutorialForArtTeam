# Quy định chung
- Nên commit thường xuyên để tránh việc mất mát (recommend ít nhất nửa ngày 1 lần)
- Team Art sẽ làm việc trên 1 nhánh riêng là nhánh **teamart**

## 1. Trước khi bắt đầu công việc
### 1.1 Chuẩn bị tool git bash 
- Vào thư mục sourcecode từ window rồi chuột phải chọn "Open Gitbash Here"

### 1.2 Check xem hiện tại có thay đổi gì ở local không 
```console 
git status 
```
- Nếu có thay đổi gì thì cần confirm lại

### 1.3 Pull code mới nhất về local
```console 
git pull origin teamart
```

## 2. Sau khi hoàn tất công việc:

### Unity
- Save (Ctrl+S) trước khi commit push / pull

### Git
#### Step 2.1: Xem danh sách những thay đổi. Bước này có thể cần phải lặp lại nhiều lần.
```console 
git status
```

#### Step 2.2: Lựa chọn những thay đổi của mình để add vào stage
- Có 2 chiến thuật để thực thi việc này:
    - Chiến thuật 1: checkout tất cả những file không cần commit, sau đó add vào stage all (nên dùng trong trường hợp số lượng file cần commit > số lượng file không cần)
        - Checkout: có thể dùng 2 lệnh này để checkout hết tất cả những file không cần commit
            ```console 
            -  git checkout <file_path> (ý nghĩa: không thay đổi file này, quay về commit gần nhất)
            -  git checkout <folder_path>/* (checkout toàn bộ các file trong thư mục)
            ```
        - Add:
            ```console 
            -  git add . (add toàn bộ những file còn lại vào stage để chuẩn bị commit)
            ```
    - Chiến thuật 2: add và commit tất cả những file cần commit vào stage, sau đó checkout all (ngược lại ở chiến thuật 1)
        - Add: có thể dùng 2 lệnh này để add hết tất cả những file cần commit vào stage
            ```console 
            -  git add <file_path> (dùng để add 1 file)
            -  git add <folder_path>/* (dùng để add các file trong 1 folder)
            ```
        - Checkout:
            ```console
            -  git checkout . (revert tất cả những file còn lại)
            ```

#### Step 2.3: Commit ở local
```console 
git commit -m "<commit_message>"
```

#### Step 2.4: Push to server
```console 
-  git pull origin teamart
-  git push origin teamart
```
