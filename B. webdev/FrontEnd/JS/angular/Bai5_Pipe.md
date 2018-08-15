# I. Pipe là gì ?
 
  - Pipe là 1 trong những hàm được tạo sẵn hoặc do người dùng tự định nghĩa để thực hiện công việc
   
   chuyển đổi cách hiển thị dữ liệu cho người dùng

# II. Sử dung pipe
  
  - {{value | pipeName : parameterl}}

# III. Custom pipe

  - `1. import {Pipe, PipeTransform} from '@angular/core'`
 
  - `2. @Pipe({name: 'LamTron'})` : Đặt tên cho pipe

  - `3. implements PipeTransform` và thực hiện phương thức `transform`
