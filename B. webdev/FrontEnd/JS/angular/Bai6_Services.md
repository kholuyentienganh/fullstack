Tìm hiểu về services trong Angular
====================================

# I. Services là gì ? 

  - Đây là 1 component để truy vấn dữ liệu được lấy từ server

  - Nó có tác dụng làm ngắn gọn code ở các component khác

# II. Hướng dẫn sử dụng

  - Lệnh `ng g s <service name>`: Để tạo 1 service

  - `import {Injectable} from '@angular/core'` : Import thư viện Injectable

  - `@Injectable({ providedIn: 'root' })` : Thực hiện inject

# III. Viết code

  - CHúng ta sẽ viết code từng method chúng ta cần ở đây. 