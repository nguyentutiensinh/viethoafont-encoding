# 🇻🇳 Font Encoding hỗ trợ Việt hóa cho FontLab

## 📝 Giới thiệu

Font chữ tiếng Việt thường đòi hỏi sự hỗ trợ đầy đủ các ký tự có dấu, dấu thanh, và các tổ hợp glyph phức tạp. Tuy nhiên, không phải phần mềm thiết kế font nào cũng cung cấp sẵn encoding phù hợp cho tiếng Việt. Vì vậy, file encoding này được tạo ra nhằm giải quyết vấn đề đó — giúp bạn dễ dàng Việt hóa font chữ trong **FontLab** một cách chính xác và hiệu quả.

Encoding này bao gồm:

- ✅ Đầy đủ **glyph tiếng Việt**: các chữ cái có dấu như ă, â, ê, ô, ơ, ư, đ...
- ✅ Hỗ trợ **dấu thanh**: sắc, huyền, hỏi, ngã, nặng dưới dạng tổ hợp glyph.
- ✅ Bao gồm **dấu câu, ký hiệu đặc biệt**, và các ký tự mở rộng Unicode.
- ✅ Được trình bày theo định dạng **12 glyph mỗi dòng**, giúp dễ kiểm tra, chỉnh sửa và đảm bảo tính nhất quán.

Việc sử dụng encoding này sẽ giúp bạn:

- 🎯 Kiểm tra nhanh font có đầy đủ glyph tiếng Việt hay chưa.
- 🎨 Thiết kế hoặc chỉnh sửa font chữ với độ chính xác cao.
- 🔍 Tránh lỗi thiếu glyph khi xuất bản hoặc sử dụng font trong môi trường thực tế.

> Đây là công cụ không thể thiếu cho bất kỳ nhà thiết kế font nào đang hướng đến việc hỗ trợ tiếng Việt chuyên nghiệp.

---

## ⚙️ Hướng dẫn cài đặt

1. **Tải file encoding** từ repository về máy.
2. **Sao chép file** vào thư mục tương ứng:

   - **macOS**:  
     `~/Library/Application Support/FontLab/FontLab 8/Encoding`
     ```
     ~/Library
        └── Application Support
          └── FontLab
              └── FontLab 8
                  └── Encoding
                      └── VHFVN.enc
     ```

   - **Windows**:  
     `C:\Users\Your_Name\AppData\Roaming\Fontlab\Encoding`
     ```
     C:\
      └── Users
          └── Your_Name
              └── AppData
                  └── Roaming
                      └── Fontlab
                          └── Encoding
                              └── VHFVN.enc

     ```

3. **Khởi động lại FontLab** để áp dụng encoding mới.

> 💡 Nếu thư mục `Encoding` chưa tồn tại, bạn có thể tự tạo thủ công.

## 📌 Lưu ý khi sử dụng encoding

- Encoding này được thiết kế riêng cho **FontLab 8** trở lên. Nếu bạn đang sử dụng phiên bản cũ hơn, một số tính năng có thể không hoạt động như mong đợi.
- Để encoding hiển thị đúng định dạng, hãy đảm bảo bảng glyph trong FontLab được thiết lập theo **12 ô mỗi dòng**.  
  👉 Bạn có thể điều chỉnh bằng cách **chuột phải vào bảng glyph**, chọn `Set Width`, sau đó nhập giá trị **12**.
- File encoding cần được lưu với định dạng `.txt` và đặt đúng vị trí trong hệ thống:
  - **macOS**: `~/Library/Application Support/FontLab/FontLab 8/Encoding`
  - **Windows**: `C:\Users\Your_Name\AppData\Roaming\Fontlab\Encoding`
- Nếu FontLab không nhận diện được encoding:
  - Kiểm tra lại tên file và phần mở rộng `.txt`
  - Đảm bảo encoding không chứa ký tự lạ hoặc khoảng trắng thừa
- Một số glyph đặc biệt yêu cầu font hỗ trợ **Unicode mở rộng**. Nếu font không có glyph tương ứng, ký tự đó sẽ không hiển thị.
- Encoding này giúp bạn kiểm tra nhanh độ đầy đủ của font tiếng Việt, tránh lỗi thiếu dấu hoặc sai tổ hợp khi xuất bản.

> ✅ Sử dụng encoding đúng cách sẽ giúp bạn tiết kiệm thời gian, tăng độ chính xác và đảm bảo chất lượng font Việt hóa chuyên nghiệp.

---

## 🔤 Cấu trúc Encoding:

### 1️⃣ Nhóm dấu và tổ hợp dấu
```
´   `   ˜   ̉   ˇ   ¯   ˚   ¨   ˛   ˙   ¸   ˝
́   ̀   ̃   ̣   ̌   ̄   ̊   ̈   ̨   ̇   ̧   ̋
ˆ   ˘   ̛   Ắ   Ằ   Ẳ   Ẵ   '   –   ~   D   Đ
̂   ̆   ̦   Ấ   Ầ   Ẩ   Ẫ   "   —   ﹅   d   đ
```

### 2️⃣ Nhóm chữ cái A/a và biến thể
```
A   Á   À   Ả   Ã   Ạ   a   á   à   ả   ã   ạ
Â   Ấ   Ầ   Ẩ   Ẫ   Ậ   â   ấ   ầ   ẩ   ẫ   ậ
Ă   Ắ   Ằ   Ẳ   Ẵ   Ặ   ă   ắ   ằ   ẳ   ẵ   ặ
```
### 3️⃣ Nhóm chữ cái E/e và biến thể
```
E   É   È   Ẻ   Ẽ   Ẹ   e   é   è   ẻ   ẽ   ẹ
Ê   Ế   Ề   Ể   Ễ   Ệ   ê   ế   ề   ể   ễ   ệ
```
### 4️⃣ Nhóm chữ cái I/i và biến thể
```
I   Í   Ì   Ỉ   Ĩ   Ị   i   í   ì   ỉ   ĩ   ị
```
### 5️⃣ Nhóm chữ cái O/o và biến thể

```
O   Ó   Ò   Ỏ   Õ   Ọ   o   ó   ò   ỏ   õ   ọ
Ô   Ố   Ồ   Ổ   Ỗ   Ộ   ô   ố   ồ   ổ   ỗ   ộ
Ơ   Ớ   Ờ   Ở   Ỡ   Ợ   ơ   ớ   ờ   ở   ỡ   ợ
```
### 6️⃣ Nhóm chữ cái U/u và biến thể

```
U   Ú   Ù   Ủ   Ũ   Ụ   u   ú   ù   ủ   ũ   ụ
Ư   Ứ   Ừ   Ử   Ữ   Ự   ư   ứ   ừ   ử   ữ   ự
```
### 7️⃣ Nhóm chữ cái Y/y và biến thể
```
Y   Ý   Ỳ   Ỷ   Ỹ   Ỵ   y   ý   ỳ   ỷ   ỹ   ỵ
```
### 8️⃣ Nhóm chữ cái cơ bản
```
B   C   F   G   H   J   K   L   M   N   P   Q
b   c   f   g   h   j   k   l   m   n   p   q
R   S   T   V   W   X   Z   1   2   3   4   5
r   s   t   v   w   x   z   6   7   8   9   0
```
### 9️⃣ Nhóm ký hiệu và dấu câu
```
!   @   #   $   %   ^   &   *   (   )   [   ]
{   }   <   >   |   /   \   ?   .   ,   :   ;
︷   ︸   -   +   _   =   〘   〙   〖   〗   〚   〛
〈   〉   《   》   「   」   【   】   〔   〕   『   』
︿   ︽   ﹁   ︻   ︹   ︵   ﹇   ﹃   ︗   “   ”   „
﹀   ︾   ﹂   ︼   ︺   ︶   ﹈   ﹄   ︘   «   »   space
```
---

## 🙏 Cảm ơn

Cảm ơn bạn đã quan tâm và sử dụng encoding này trong quá trình Việt hóa font chữ với FontLab. Dự án được xây dựng với mong muốn hỗ trợ cộng đồng thiết kế font tại Việt Nam có một công cụ đơn giản, hiệu quả và dễ triển khai.

Hy vọng encoding này sẽ giúp bạn:

- Tiết kiệm thời gian kiểm tra và chỉnh sửa glyph tiếng Việt
- Nâng cao độ chính xác khi thiết kế font hỗ trợ Unicode
- Tạo ra những sản phẩm font chất lượng, thân thiện với người dùng Việt

Nếu bạn có góp ý, phát hiện lỗi, hoặc muốn đóng góp thêm, hãy ghé thăm repository tại:

**[github.com/nguyentutiensinh/viethoafont-encoding](https://github.com/nguyentutiensinh/viethoafont-encoding)**

> Mọi đóng góp đều được trân trọng.  
> Chúc bạn thiết kế được những bộ font thật đẹp và chuẩn Việt 💙








