# HTML CSS 
## Thẻ meta.
- Thẻ ```<meta>``` dùng để cung cấp thêm "thông tin về trang web" cho trình duyệt và các công cụ tìm kiếm (những thông tin này không hiển thị lên màn hình, tuy nhiên trình duyệt và các công cụ tìm kiếm có thể đọc và hiểu được).
- Thuộc tính charset dùng để xác định kiểu mã hóa ký tự của trang web.
- Tiếng Việt của chúng ta sử dụng kiểu mã hóa ký tự là UTF-8 ```<meta charset="UTF-8">```.
- 
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
- Tag ```<article>``` định nghĩa một bài viết, một nội dung riêng biệt. Thường được sử dụng trong:

     - Tin tức.
     - Comment.
     - Nội dung quảng cáo.
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

### Gradient : đổ từ màu này sang màu kia
- Set gradient cho background ```background-image: linear-gradient(direction,color1,color2)```.

### Sự khác nhau giữa opacity visibility và display none.
- Đầu tiên sử dụng ```curson: pointer```.
- Độ mờ ```opacity:0``` chạy từ 0->1.Nếu ```0``` ẩn đi nhưng vẫn chiếm diện tích, ấn vào được(transition,nhấn vào hiện ra,hiệu ứng).
- ```visibility:hidden``` chiếm diện tích nhưng k ấn vào được(transition,nhấn vào hiện ra,hiệu ứng).
- ```display:none``` ẩn đi và không chiếm diện tích.

### Shadow : tạo độ bóng 
- 

### Độ ưu tiên

### Child selector 

### Type selector 
- Lấy theo kiểu chứ không phải vị trí như children.
```html
<ul>
     <p>loret</p>
     <li>1</li>
</ul>
```
- Child sẽ k hỉu first là ```li``` và nó k thực thi. Còn type thì hiểu.
### Combinators
- ```+``` : trỏ đến thẻ liền tiếp phía sau, cùng cấp.
- Ví dụ : 
```html
<p>hello</p>
<span>hi</span>
```
trong css sẽ là 
```css
p + span {
     color: #000;
}
```
thì màu #000 sẽ được áp dụng cho thẻ ```span```.

- ```~``` : chỉ cần là thẻ cùng cấp ở sau.

### Selector nâng cao trong CSS
- Bắt đầu : 
```
a[attribute^="..."] {
       //body;
}
```
- Kết thúc : 
```
a[attribute$="..."] {
       //body;
}
```
- Chỉ cần có ... : 
```
a[attribute*="..."] {
       //body;
}
```

- Chính xác :  ```=```.

[Thực thi thẻ html tại đây ](html/selectorHigh.html) .
[Thực thi thẻ css tại đây ](css/sel.css) .

### Transition
- Hiệu ứng chuyển đổi mượt mà giữa các trạng thái của một phần tử khi có sự thay đổi trong thuộc tính CSS.

```css
transition: all 2s linear;
```
[Thực thi tại đây ](css/child.css) .

### Transform
- Thay đổi vật thể ban đầu nhưng vẫn chiếm diện tích như vậy.
- Không ảnh hưởng đến vật khác , bản chất nó chỉ đè lên vật khác.
- Mở rộng chiều dài và chiều cao : 
```css
transform: scale scaleX() scaleY();
```
- Muốn quay bao nhiêu độ thì dùng :
```css
transform: rotate(34deg)
```

- Có rotateX và rotateY và còn có rotateZ ( xoay theo mặt phẳng).
- Di chuyển trái phải thì dùng ```translateX```, còn trên dưới thì dùng ```translateY```.
- Trong ```translate``` có thể điền %, biểu thì cho bao nhiêu % so với kích thước của vật được translate.
> Tổng hợp : transform: scale(x,y) rotate(ndeg) translate(X,Y).
- Nghiêng thì dùng ```skew```.

### Position 
#### Fixed Position
- Cố định luôn và chỉ phụ thuộc vào thẻ body .
- Không nên đi kèm với transform.
### Before và after: điền vào trước và sau.
- Thêm 1 dấu tròn nhỏ ở trước hoặc sau.
[Thực thi tại đây ](css/dot.css) .
- Line nằm giữa text (---text---).
- Text sẽ được bỏ trong 1 thẻ như là thẻ ```span``` ở bên trong 1 thẻ sử dụng line như ```h3```.
[Thực thi tại đây ](css/dot.css) .
- Làm icon và 1 bg mờ ở dưới .
     - Để background ở dưới icon cùng màu với icon hay là text mà cần giảm độ mờ thì dùng ```background-color: currentColor;``` sẽ theo màu đó và kết hợp với ```opacity:n``` n là từ 0->1 ( độ mờ của background ).

#### Hiệu ứng khi hover

       
