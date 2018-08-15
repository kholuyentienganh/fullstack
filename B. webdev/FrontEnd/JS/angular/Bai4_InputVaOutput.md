# I. Input

 - Trong quá trình tái sử dụng các component chúng ta cần phải sử dụng các tham số cho component đó để dữ
 
 liệu được tạo ra là không trùng khớp

 - Sử dụng Input là 1 điều tuyệt vời để thực hiện điều đó

 - Đầu tiên cần phải import  Input vào chỗ .ts

 - Sau đó `@Input() name : String` được đặt ở trong class. Nó có nghĩa là name được lấy từ tham số truyền 
 
 vào cho component và có kiểu String

 - Có thể phố hợp vơi ngFor để tạo ra hàng loạt component khác nhau để geder dữ liệu

# II. Output
  
  - Trong trường hợp ta có 2 component `parent` và `child`

  - Nếu như ở child có nút add, và parent có nơi hiển thị các value. Khi nhất add ở child thì parent tăng lên

  - Sử dụng `Ouput` và `EventEmitter` là 1 ý tưởng tuyệt vời

  - Quá trình thực hiện như sau:
    
    + `Output, EventEmitter` : import vào child

    + `<app-child (myclick)="value = value +1"></app-child>` : Cái này sẽ nằm ở giao diện của parent.
      
       - myclick và tên do mình tự đặt. value là biến ở trong parent

    + `@Output() myclick = new EventEmitter();` Sử dụng out ở child

    + `<button (click)="addForParent()">Add</button>`: Thêm sự kiện cho nút ở child

    +  `this.myclick.emit();` : Là phần thân hàm của `addForParent()`

    + Chúng ta có thể sử dụng thêm tham số cho Ouput như sau:

      - `<app-child (myclick)="changeValue($event)"></app-child>` : Truyền cho anh này 1 giá trị event

      - `this.myclick.emit(true);` : Ở emit truyền vào tham số cần thiết

