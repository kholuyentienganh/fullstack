Directive và ngStyle
==============================

# I. Giới thiệu cơ bản về directive và ngStyle

# 1. Directive là gì ?

  - Đưa ra các chỉ dẫn để Angular chuyển đổi template thành DOM

# 2. Phân loại

  - Component : Directive với 1 template

  - Attribute Directive: THay đổi việc hiển thi hoặc hành vi của DOM, component hoặc các Directive khác

  - Structural directive : Thường thêm bớt các DOM

# II. ngStyle và ngClass (Attribute Directive)

  - `[ngStyle]="name.length % 2 === 0 ? evenStyle: oddStyle"`
 
  - `[ngStyle]` : là đánh dấu ngStyle

  -  `evenStyle` và `oddStyle` : là 1 obj của js. 
 
  - evenStyle = {color: 'red', fontSize: '23px'}

  - oddStyle = {color: 'black', fontSize: '23px'}

# III. ngIF và ngFor (Structural directive)

  - `*ngIf= condition`: Đây là cú pháp của angular về ngIf. 

  - Nó được sử dụng để diễn tả 1 tag html được hiển thị hay không hiển thị

  - `*ngFor="forEach"`: 

  - Nó được sử dụng để duyệt các phần tử được thực hiện bởi forEach

