- cung cấp  _./_
- truy xuất ra ngoài 1 cấp _../_
- thuộc tính _attibute_
- Thẻ _tag_
- CSS nó sẽ chạy từ trên xuống, nếu có hai đoạn code cùng thực hiện 1 chức năng thì nó sẽ ưu tiên đoạn code ở dưới
- _div_ là thẻ block, có độ rộng 100% phần tử chứa nó, lưu ý: chưa nói tới vấn đề khi sử dụng với CSS
- _div_ thường được dùng rất nhiều, khi chứa layout, gom 1 khối nào đó
- _img_ là thẻ inline, tự đóng, dùng để hiển thị hình ảnh với hai thuộc tính là `src` và `alt`
- _alt_ viết tắt của `alternate text` nó dùng trong việc SEO, khi hình ảnh bị lỗi hoăcj sai đường dẫn thì _alt_ sẽ hiển thị để người dùng biết hình ảnh đó nói gì về cái gì
- _span_ là thẻ inline, nó thường dùng cho những đoạn chữ ngắn 
- _class_ là thuộc tính dùng để sử dụng các class cho thẻ, sau đó dùng để styles trong css
- việc đặt tên class khá nan giản, khó, không nên đặt tên tiếng việt, nên đặt tên tiếng anh ngắn gọn dễ hiểu
- Thẻ tiêu đề : h1, h2, h3, h4, h5, h6
- _h1_: Môĩ trang chỉ có tối đa 1 thẻ h1 mà thôi, thẻ này thường được dùng cho những tiêu đề lớn của trang
- _h2_: Dùng được nhiều, thường được dùng cho những block nhỏ 
- _h4,h5,h6_: Tương ứng cho những tiêu đề nhỏ hơn
- Thẻ _a_: Là thẻ inline, chắc chắn là dùng cho thẻ liên kết, nó có 3 thuộc tính hay dùng `href`, `target`, và `rel`
- Khi dùng `target` có giá trị là `blank` thì thẻ a nên thêm thuộc tính `rel="noopener noreferrer"`
- _Fonts chữ:_
-1. sẽ có sẵn ở Google Fonts
-2.Không có ở Google Fonts mà được mua, tải trên mạng về máy
- _font-weight_: Đỗ đậm nhạt của chữ , 100-> 900, normal, bold, bolder, extra bold, light, thin, regular, medium, semibold
-_font-family_: Thiết lập font chữ, truyền vào là font name(tên của font chữ)
- `sans-serif`: Chữ không có chân
- `serif`: Chữ có chân
- CSS Selectors: tag, class, id, attribute
- Tags: h1, h2, h3, div, body, span, a
Class: .name, .tour, .tour-header
-Id: #headeer, #content
- Attribute: Late `*`
- Special selector: \* _chonj toàn bộ selector_
- Cấu trúc 1 đoạn code CSS
cssSelector{
    property: value;
}
h1,.name,#header, input[type='email']{
    font-family: 'Inter'
}
- _User Agent Stylesheet_ : CSS mặc định của trình duyệt, mỗi trình duyệt sẽ có CSS mặc định khác nhau 
- _CSS reset_ : DÙng để reset CSS mặc đinh của các trình duyệt, và 'bắt buộc' phải có
- _box-sizing_: margin, padding, border, width, height, đơn vị px
- _width_ : Độ rộng
- _height_: Chiều cao
- _border_ : Viền
_color_: Màu chữ
_background-color_:Màu nền
- _Mã màu_ : hexa(#ffa400), orange,rgb(0,0,0), rgba(0,0,0,0.5)
- _Alpha_ (opacity): 0 -> 1
- **box-sizing**
- _content-box_: Độ rộng lúc này của 1 khối sẽ bao gồm width + padding(left+ right )+ border (left+right)
- _border-box_: Độ rông lúc này của 1 khối sẽ bao gồm padding và border, nên áp dụng cho toàn bộ selector (\*)
- _width_:Độ rộng
- _height_: Chiều cao
- _border_: viền
- _shorthand_: Viết rút gọn
- _padding_: KHông thể dùng số âm
- _margin_: Có thể dùng số âm, có giá trị `auto`
- Đơn vị : px, em , rem, vw, vh, %
-  _text-decoration_: Gạch dưới của thẻ a, 
`none`,`underline`, `overline`, `line-through`
-_border-radius_: Độ bo góc của khối,  càng lớn thì càng bo góc, neeus hình vuông mà bo góc lớn thì sẽ tạo ra honhf tròn, còn nếu là hình chữ nhật có bo góc lớn thì sẽ tạo ra hình elip.
- border-top-left-radius,border-top-right-radius ,
border-bottom-left-radius, border-bottom-right-radius.
- _line-height_: Khoảng cách giữa các dòng chữ
- Khi những thẻ inline nằm cạnh nhau thì nó sẽ nằm trên 1 hàng, ngược lại những thẻ block thì nó sẽ tạo ra hàng mới. 
- _display_: block, inline, inline-block, none, flex, grid.
- `block` : Biến thành thẻ block
- `inline` : Biến thành thẻ inline, nó sẽ bị hạn chế vài thuộc tính CSS liên quan tới box-sizing như là padding-top, padding-bottom
- `inline-block` : Biến thành thẻ inline-block, là sự kết hợp giữa inline và block, khi các thẻ có thuộc tính inline-block nó sẽ kế thừa đặc tính của inline tức là nằm cạnh nhau thì sẽ nằm trên 1 hàng, có độ rộng bằng nội dung nó chứa, không bị hạn chế CSS
- `none` : Ẩn luôn, không thấy được
- `flex`: Dùng rất nhiều hiện nay, nếu master được nó thì code layout vô tư hihi
- _min-width_:Độ rông tối thiểu , ví dụ 100px -> >= 100px
- _max-width_:Độ rộng tối đa, ví dụ 100px -> <=100px
- _flexbox_: Áp dụng thuộc tính display: flex vào phần tử mình muốn dàn layout
- _cacl_: Hàm dùng để tính toán, + - * / , lưu ý phải có khoảng cách giữa các phép tính 
- _component_: Mục đích là tái sử dụng và có thể tùy chỉnh 1 chỗ để sử dụng nhiều nơi
- _column-gap_: Khoảng trống chiều dọc
- _row-gap_: Khoảng trống chiều ngang

- _pug_
---
//_align-items_ :Align Items là một trong những thuộc tính quan trọng của Flexbox và Grid Layout, dùng để căn chỉnh phần tử con bên trong một container theo trục chính (main axis) của flexbox. Thuộc tính này thường được sử dụng với display: flex để định dạng flexbox.
- `flex-start`: Căn chỉnh các phần tử con tới đầu của container.
- `flex-end`: Căn chỉnh các phần tử con tới cuối của container.
- `center`: Căn chỉnh các phần tử con vào giữa của container.
- `stretch`: Kéo các phần tử con để chúng phù hợp với kích thước của container.
- `baseline`: Căn chỉnh các phần tử con tới đường cơ sở (baseline) của container.
/*.container {
  display: flex;
  align-items: center; /* căn chỉnh các phần tử con vào giữa theo trục chéo */
}*/
*Trục chéo (cross axis): Là trục vuông góc với trục chính, chạy qua chiều rộng (width) của container trong Flexbox và Grid Layout.*
*Ví dụ, trong một container dùng `Flexbox` với `flex-direction: row`;, trục chính sẽ là theo `chiều ngang`, còn `trục chéo sẽ là `theo chiều `dọc`. Ngược lại, nếu` flex-direction` được thiết lập là `column`, thì `trục chính sẽ `là theo` chiều dọc` và `trục chéo` sẽ là theo `chiều ngang`.*
**flex-wrap**
- Thuộc tính CSS đặt xem các mục linh hoạt có bị ép buộc trên một dòng hay có thể nằm trên nhiều dòng hay không. Nếu cho phép ngắt dòng, nó sẽ đặt hướng các dòng được xếp chồng lên nhau.flex-wrap
- _flex-wrap: nowrap;_   Item One     Item Two    Item Three    Item Four   Item Five   Item Six
- Các mục linh hoạt được trình bày trên một dòng duy nhất có thể khiến vùng chứa linh hoạt bị tràn. Bắt đầu chéo tương đương `cross-star` với bắt đầu hoặc trước tùy thuộc vào flex-direction giá trị. Đây là giá trị mặc định.

- _flex-wrap: wrap;_ Item One    Item Two    Item Three
                     Item Four   Item Five   Item Six
- Các mục linh hoạt chia thành nhiều dòng. Bắt đầu chéo tương đương với bắt đầu hoặc trước giá trị tùy thuộc flex-directionvà kết thúc chéo ngược lại với bắt đầu chéo được chỉ định .
-_flex-wrap: wrap-reverse;_  Item four    Item five    Item six
                             Item One     Item two       Item three 
- 
Hoạt động tương tự wrapnhưng bắt đầu chéo và kết thúc chéo được hoán vị.
- _component_: Mục đích tái sử dụng và có thể tùy chỉnh một chỗ để sử dụng nhiều nơi
- _pug_: 
- _mixins_: Giống function trong javascript mục đích là tái sử dụng code
- Biến : = , #{biến}

- _position_ : có 5 giá trị chính : static, relative, absolute, sticky, fixed
- _relative_ : khi sử dụng giá trị này thì phải lưu ý xem phần tử con của nó có sử dụng position là `absolute` hay không ?
- _absolute_:KHi sử dụng giá trị này thì phải lưu ý xem phần tử chứa nó gần nhất có sử dụng position là absolute hay relative không?
- _responsive_ : 
- _breakpoints_: 320px, 380px, 768px 1024px 1200 1366 1220 1600 1920
- _min-width_:
- _max-width_:
-_media queries_:
`/* @media screen and (min-width: breakpoints){}*/`
`@media screen and (min-width: 320px){}`
`@media screen and (max-width: breakpoints -1px)`
`@media screen and (max-width: breakpoints -0.02px) nên làm theo cái này`
`@media screen and (max-width: 1023.98px){}`
- _transform_: translate(translateX(value)  translateY(value)), skew(skewX, skewY), rorate(rorateX,,Y,Z), scale(X, Y);
-`translateX` : Nếu giá trị là số dương thì nó sẽ di chuyển qua bên phải, ngược lại thì di chuyển qua bên trái.
- `translateY`: Nếu giá trị là số dương thì nó đi xuống, ngược lại nó sẽ đi lên
- `value`: 10px ; 20px; -15px; -30px , 10%, lưu ý khi sử dụng % thì % ở đây chính là độ rộng hoặc chiều cao của khối chúng ta đang áp dụng thuộc tính transform và hàm translate
- _variables_: Biến là gì? Khai báo như thế nào ? Cách sử dụng ra sao ? Ưu và nhược điểm của nó là gì ?
- _grid_: dàn layout cực nhanh

**Để thụt lề tất cả các dòng code vào hoặc ra một tab trong Visual Studio Code, bạn có thể sử dụng các phím tắt sau:**

- `Để thụt lề vào: Chọn các dòng bạn muốn thụt lề và nhấn Ctrl + ].`
- `Để thụt lề ra: Chọn các dòng bạn muốn thụt lề và nhấn Ctrl + [.`
- `Nếu bạn muốn định dạng một phần của code thay vì chỉ thụt lề, bạn có thể chọn các dòng và sử dụng Ctrl + K, sau đó Ctrl + F để định dạng1.`
- _grid_ : Dàn layout cực nhanh
- _time_ : nó là thẻ inline
- _each in pug_ : dùng để duyệt qua danh sách các phần tử trong mảng để hiện thị
- _object-fit_ : Thuộc tính này dùng cho thẻ img hoặc video , mục đích là để hiện thị hình ảnh hoặc video vừa khung chứa nó hay không?
- _object-position_: Dùng để căn chỉnh vị trí hiện thị của img hoặc video khi dùng với thuộc tính
- _css selectors child_: :nth-child(number), nth-last-child(number), :first-child , :last-child, những phần tử cùng cấp, 
.gem-item:first-child, .gem-item:last-child, .gem-item:nth-child(5), :not(selectors), .gem-item:not(first-child), .gem-item:not(:nth-child(5));
- _width: fit-content_: có độ rộng bằng với nội dụng nó chứa
- _margin-inline_ : tương ứng margin-left và margin-right
- _padding-inline_ : tương ứng padding-left và padding-right
- _margin-block_ : tương ứng margin-top và margin-bottom
- _padding-block_ : tương ứng padding-top và padding-bottom
-_caniuse_: là một trang web giúp chúng ta kiểm tra những thuộc tính trong css xem nó có được nhiều trình duyệt hỗ trợ hay không? Từ đó chúng ta có thể chắc chắn sử dụng vào dự án 
-_semantic tags_:header(phần phía trên) , footer(phía dưới), main(chính), section(khối), article(một bài viết), nav(menu), aside(phần bên trái bấm chạy ra chạy vô)
