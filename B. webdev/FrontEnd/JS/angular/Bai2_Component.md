Hướng dẫn cơ bản về component
===========================

# I. Component là gì ?

   - Điều chỉnh một phần của màn hình (view)

   - Component có thể chứa nhiều thẻ HTML

   - Component có thể chứa nhiều component khác

   - Component có thể nhận tham số

   - Component có thể rất linh hoạt

# II. Lợi ích của việc sử dụng component 

   - Dể quản lý code

   - Tái sử dụng code

# III. Tạo và sử dụng component

   - Tạo với câu lệnh `ng g c <component-name>`

   - Sau khi sử dụng câu lệnh trên. Một thư mục được tạo ra với các file liên quan tới component

   - Tạo đây chúng ta đã tạo được 1 html tag như sau: `<component-name></component-name>`. Với tag  này có thể hiển thị toàn bộ dữ liệu cho component vừa được tạo ra

# IV. Binding data

  - `{{value}}` : value binding 

  - `[property] = "value"` : property binding 

  - `(event) = "handler"` : event binding

  - `[(ng-model)] = "property"` : binding hai chiều

# V . Binding 2 chiều
 
  - Import thư viện:
    
     + Import thư viện `FormModule` từ trong `@angular/forms`

# VI.  Style binding và class binding

  - Style binding : `[style.color]="name.length %2 ===0 ? 'red':'blue'"` : Trong đó
    
    + [style.color] : giá trị cần binding

    + name là 1 biến được tạo ra từ Binding 2 chiều
  
  - class binding:

    + Thiết lập 2 class css red và blue trong file .css
 
    + `[class]="isHighlight? 'blue':'red'"` trong đó:
      
      - [class] : class binding

      - isHighlight : 1 biến ở ts
