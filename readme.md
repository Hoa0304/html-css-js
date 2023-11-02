# HTML CSS 
## Thẻ cơ bản.
- ```div``` : thẻ bao bọc 1 khối gì đó.
- ```p``` : chứa những đoạn văn dài(thẻ block) .
- ```h1``` : thẻ tiêu đề , mỗi một web chỉ có duy nhất 1 thẻ ```h1``` (thẻ block) .
## Thẻ inline.
- ```<a href="">b</a>``` : thẻ link, __href__ : là thuộc tính và nó chứa đường link của ```b``` .
     - Nếu muốn mở sang 1 tab mới mà không ở trong cùng 1 trang thì dùng thuộc tính ```target``` :
     ```<a href="https://github.com/Hoa0304" target="_blank" rel="noopener noreferrer">CamHoa</a>```.
         - Trong gg khuyến khích nếu dùng target thì nên dùng thêm ```rel``` : giúp chúng ta về phần bảo mật.
- ```<img src="" alt="" />``` : Thẻ ảnh , ```src``` : đường link ảnh , ```alt``` : khi ảnh không thực hiện thì sẽ hiển thị chữ trong alt.

## Thẻ danh sách.
 
### Thẻ danh sách có thứ tự.

```html
    <ol>
        <li>Hi</li>
        <li>Hello</li>
        <li>Bye</li>
        <li>Bai</li>
    </ol>
```
- ```ol``` : in ra số thứ tự , kqua trên sẽ cho ra là ```1.Hi, 2.Hello, 3.Bye, 4.Bai``` .

### Thẻ danh sách không có thứ tự.

```html
    <ul>
        <li>Hi</li>
        <li>Hello</li>
        <li>Bye</li>
        <li>Bai</li>
    </ul>
```
- ```ul``` : in ra dấu chấm  như bên trái .

## Thẻ sematic : làm cho code gọn gàn hơn , cấu trúc mạch lạc hơn , dễ hiểu hơn.

- Thẻ ```header``` : thanh ngang trên đầu trang web.
- Thẻ ```footer``` : thanh ngang dưới trang web.
- Thẻ ```aside``` : thanh dọc 2 bên .
- Thẻ ```nav``` : menu.
- Thẻ ```main``` : chứa nội dung chính.
- Thẻ ```section``` :  có thể chứa tiêu đề, đoạn văn bản, hình ảnh, hoặc các phần tử khác. Việc sử dụng ```<section>``` giúp cho việc đánh dấu các phần quan trọng trên trang web và giúp các công cụ tìm kiếm và trình đọc màn hình hiểu được cấu trúc nội dung của trang một cách tốt hơn.
     - Trong thẻ ```section``` chứa thẻ ```article``` : 1 bài viết.

## Thẻ inline.

- Thẻ ```iframe``` : cho phép nhúng video.
- Thẻ ```span``` : chứa dòng chữ ngắn.
- Thẻ in đậm : ```strong``` và ```b``` .
- Thẻ in nghiêng : ```em``` và ```i``` .

> Vào đường link này xem thẻ inline và thẻ block : {htmlreference.io} .

## Thẻ inline và thẻ block khác gì nhau?
- Thẻ inline :
     - Có độ rộng bằng nội dung chứa nó.
     - Nếu có nhiều thẻ inline nằm vs nhau thì nó sẽ nằm trên 1 hàng.
     - Bị hạn chế về CSS.
- Thẻ block :
     - Có độ rộng = thẻ cha chứa nó .
     - Nếu nhìu thẻ block nằm với nhau thì nó sẽ xuống hàng.
## Sự khác nhau giữa class và id :
- Class :
     - Có thể trùng nhau, sử dụng cho nhiều phần tử giống nhau.
- ID :
     - Duy nhất, k dc đặt trùng nhau.
     - sử dụng cho Form hay là input.

## Quy tắc BEM : Block Element Modifier
- Block : laptop.
- Element : mouse,screen,keyboard.
- Modifier for block : big, small.
- Modifier for element : small screen, small keyboard.
- Cú pháp :
     -  ```Block__Element--modifier```.
     - ```Block--modifier```.
     - ```Block__Element```.

- Eg :
     - laptop__keyboard , laptop__touchpad.
     - laptop--small, laptop--expensive.
     - laptop__touchpad--smooth.

[Thực hành nèo ](html/bem.html) 

## Emmet 
- Để di chuyển giữa các dòng : ```alt``` + mũi tên lên xún .
- Tạo 1 cái giống cái trên : shift +alt + mũi tên xún.
- Đổi tên tất cả cùng 1 tên : ấn vào cúi tên rồi nhấn ```ctrl``` + D.
- Tạo ra 10 cái có cùng nội dung : ```ul>li*10{Hoane}``` .
- Tạo ra chạy số theo thứ tự : ```ul>li*10{$}``` .
- Tạo ra 10 cái có cùng tên : ```ul>li.Hoane*10``` .
- Dấu ```+``` : tạo ra những thẻ có cùng cấp với nhau .
- Dấu ```^``` : tạo ra thẻ mà như ```cd ..``` (thoát 1 folder) .

## CSS Reset
- Lên trình duyệt khác nhau sẽ hiển thị khác nhau.
## Thuộc tính CSS 
[Thực hành nèo ](html/css.html) 

### Thuộc tính color
```rgba(0,0,0,0.1)``` : giảm độ mờ (0->1).
### Các thuộc tính về kích thước
- Nếu bị tràn muốn ẩn đi thì use : ```overflow: hidden```.
- Nếu bị tràn muốn sroll ( kéo xuống ) : ```overflow-y : auto```.
- Nếu nội dung quá dài thì tự cao lên , thay vì dùng ```height``` thì dùng ```min-height```.
### Các thuộc tính về background
- Để chèn 1 hình làm backgroudn dùng : 
```html
background-image: url(...);
width :100%;
height:100px;
```
     - Lúc này background sẽ bị tràn màn hình.
     - Nếu muốn background nằm ở trung tâm thì dùng :
```background-position: center center```.
     - Nếu muốn phủ hết thì dùng ```background-size: cover``` .
     - Nếu muốn không bị lặp lại thì dùng ```background-repeat: no-repeat```.
     - Nếu muốn scroll vẫn đứng yên thì dùng ```background-attachment: fixed```(cố định ở 1 vị trí).
- Cách để viết gọn hơn :
```html
background: red url() no-repeat center center / cover;
```
> Khi làm background cần phải xét height và width.

### Các đơn vị hay dùng
- % : chạy theo phần tử cha chứa nó.
- vw : không care ai ( áp dụng background để không bị scroll).
- px : cố định .
- em : phụ thuộc vào thuộc tính font-size của chính nó hoặc phần tử chứa nó.
- rem : phụ thuộc vào thuộc tính font-size của thẻ html.

### Thuộc tính border : viền bao bọc 
- Có 2 cách viết :
     - Cách 1 : 
          ```css
          border: 2px solid black;
          ``` 
     - Cách 2 : 
     ```css
         border-width: 2px;
         border-style: solid;
         border-color: black;
     ```
> Ngoài ra còn có border-top, border-right, and border-bottom, border-left.

- Có 3 loại border-style :
     - Solid : đường viền liền .
     - dotted : đường viền ```....```.
     - dashed : đường viền ```----```.

__Outline cũng giống border, nhưng border có thể radius còn outlined thì không__

### Thuộc tính margin : tạo khoảng trống bên ngoài
    - trên dưới / trái phải.
    - trên / trái phải / dưới.
    - trên / phải / dưới / trái.
### Thuộc tính padding: tạo khoảng trống bên trong

>> Note : Margin có thể dùng số âm còn padding thì không thể.

### Box-sizing : khuyên nên dùng cho cả trang web
- Gía trị mặc định :
```css
box-sizing: content-box;
```
- Có nghĩa là :
     - width = width + padding-left + padding-right + border-left + border-right.
     - height = height + padding-top + padding-bottom + border-top + border-bottom.

- Nếu dùng ```box-sizing: border-box;``` thì cái border và padding cũng sẽ nằm trong width và height.

- Có nghĩa là :
     - width = width - padding-left - padding-right - border-left - border-right.
     - height = height - padding-top - padding-bottom - border-top - border-bottom.

### Thuộc tính display : none - dùng khi res

- Eg: ```<a href="#">CHTran</a>```.

- Không dùng underline ```text-decoration: none;```.

### Thuộc tính về font 
 - Độ đậm nhạt của chữ ```font-weight``` - mặc định là 400.
 - Để chữ to hơn ```font-size```.
 - Nếu muốn chữ in nghiêng ```font-style: italic```.
 - Khoảng trống cách ra giữa 2 dòng```lineheight``` mặc định là 1.
 - Gía trị mặc định là chữ sẽ nằm bên trái, nếu muốn sang phải thì dùng ```text-align: right```. Muốn ở giữa thì thay ```right``` thành ```center```. Còn canh đều 2 bên dùng ```justify```.
 - Khoảng cách giữa các ký tự ```letter-spacing```.
 - Khoảng cách giữa các từ ```word-spacing```.
 - Muốn all chữ hiển thị trên 1 dòng ```white-space: nowrap```.
     - Nếu chữ quá dài thì sẽ hiển thị dấu 3 chấm :
          - Đầu tiên : ```overflow: hidden```- nếu tràn ra ngoài thì sẽ ẩn đi.
          - Tiếp theo : ```text-overflow: ellipsis```- hiển thị dấu 3 chấm.
- Hiển thị dấu 3 chấm trên hàng thứ 3 :
     ```css
     display: -webkit-box;
     -webkit-box-orient: vertical;
     -webkit-box-line: 3;
     overflow: hidden;
     text-overflow: ellipsis;
     ```
     - ```-webkit-box-line: 3;``` ở số 3 thì mình muốn ở dòng thứ mấy hiển thị thì nhập vào vị trí số hàng đó.
- Truyền vào là 1 chữ , spam thì để tự động xuống dòng tùm lum ```word-break: break-all;``` và ```break-word``` cho tự đống xuống hàng theo chữ.
### Các thuộc tính cho hình ảnh
### Các pseudo cơ bản
- Khi rê chuột vào ```:hover```.
- Khi nhấn vào ```:active```.
- Khi đã nhấn rồi ```:visited```.