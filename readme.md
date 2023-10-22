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