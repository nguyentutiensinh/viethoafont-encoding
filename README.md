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
## 📝 Danh Sách unicode hỗ trợ

STT | Char | Unicode | Name
-- | -- | -- | --
1 | – | uni00CA | endash
2 | ́ | uni0301 | acutecomb
3 | ̀ | uni0300 | gravecomb
4 | ̉ | uni0309 | hookabovecomb
5 | ̃ | uni0303 | tildecomb
6 | ̣ | uni0323 | dotbelowcomb
7 | ̆ | uni0306 | brevecomb
8 | ̂ | uni0302 | circumflexcomb
9 | ̛ | uni031B | horncomb
10 | Ư< | uni031B.ss02 | uni031B.ss02
11 | ‘ | uni2018 | quoteleft
12 | … | uni2026 | uni2026
13 | — | uni0049 | emdash
14 | ´ | uni00B4 | acute
15 | ` | uni0060 | grave
16 | ̉ | uni0309.case | hookabovecomb.case
17 | ˜ | uni02DC | tilde
18 | ̣ | uni0323.case | dotbelowcomb.case
19 | ˘ | uni02D8 | breve
20 | ˆ | uni02C6 | circumflex
21 | U< | uni031B.ss01 | uni031B.ss01
22 | ư< | uni031B.ss03 | uni031B.ss03
23 | ’ | uni2019 | quoteright
24 | ︙ | uniFE19 | uniFE19
25 | A | uni0041 | A
26 | Á | uni00C1 | Aacute
27 | À | uni00C0 | Agrave
28 | Ả | uni1EA2 | Ahoi
29 | Ã | uni00C3 | Atilde
30 | Ạ | uni1EA0 | Adotbelow
31 | a | uni0061 | a
32 | á | uni00E1 | aacute
33 | à | uni00E0 | agrave
34 | ả | uni1EA3 | ahoi
35 | ã | uni00E3 | atilde
36 | ạ | uni1EA1 | adotbelow
37 | Â | uni00C2 | Acircumflex
38 | Ấ | uni1EA4 | Acircumflexacute
39 | Ầ | uni1EA6 | Acircumflexgrave
40 | Ẩ | uni1EA8 | Acircumflexhoi
41 | Ẫ | uni1EAA | Acircumflextilde
42 | Ậ | uni1EAC | Acircumflexdotbelow
43 | â | uni00E2 | acircumflex
44 | ấ | uni1EA5 | acircumflexacute
45 | ầ | uni1EA7 | acircumflexgrave
46 | ẩ | uni1EA9 | acircumflexhoi
47 | ẫ | uni1EAB | acircumflextilde
48 | ậ | uni1EAD | acircumflexdotbelow
49 | Ă | uni0102 | Abreve
50 | Ắ | uni1EAE | Abreveacute
51 | Ằ | uni1EB0 | Abrevegrave
52 | Ẳ | uni1EB2 | Abrevehoi
53 | Ẵ | uni1EB4 | Abrevetilde
54 | Ặ | uni1EB6 | Abrevedotbelow
55 | ă | uni0103 | abreve
56 | ắ | uni1EAF | abreveacute
57 | ằ | uni1EB1 | abrevegrave
58 | ẳ | uni1EB3 | abrevehoi
59 | ẵ | uni1EB5 | abrevetilde
60 | ặ | uni1EB7 | abrevedotbelow
61 | E | uni0045 | E
62 | É | uni00C9 | Eacute
63 | È | uni00C8 | Egrave
64 | Ẻ | uni1EBA | Ehoi
65 | Ẽ | uni1EBC | Etilde
66 | Ẹ | uni1EB8 | Edotbelow
67 | e | uni0065 | e
68 | é | uni00E9 | eacute
69 | è | uni00E8 | egrave
70 | ẻ | uni1EBB | ehoi
71 | ẽ | uni1EBD | etilde
72 | ẹ | uni1EB9 | edotbelow
73 | Ê | uni00CA | Ecircumflex
74 | Ế | uni1EBE | Ecircumflexacute
75 | Ề | uni1EC0 | Ecircumflexgrave
76 | Ể | uni1EC2 | Ecircumflexhoi
77 | Ễ | uni1EC4 | Ecircumflextilde
78 | Ệ | uni1EC6 | Ecircumflexdotbelow
79 | ê | uni00EA | ecircumflex
80 | ế | uni1EBF | ecircumflexacute
81 | ề | uni1EC1 | ecircumflexgrave
82 | ể | uni1EC3 | ecircumflexhoi
83 | ễ | uni1EC5 | ecircumflextilde
84 | ệ | uni1EC7 | ecircumflexdotbelow
85 | I | uni0049 | I
86 | Í | uni00CD | Iacute
87 | Ì | uni00CC | Igrave
88 | Ỉ | uni1EC8 | Ihoi
89 | Ĩ | uni0128 | Itilde
90 | Ị | uni1ECA | Idotbelow
91 | i | uni0069 | i
92 | í | uni00ED | iacute
93 | ì | uni00EC | igrave
94 | ỉ | uni1EC9 | ihoi
95 | ĩ | uni0129 | itilde
96 | ị | uni1ECB | idotbelow
97 | O | uni004F | O
98 | Ó | uni00D3 | Oacute
99 | Ò | uni00D2 | Ograve
100 | Ỏ | uni1ECE | Ohoi
101 | Õ | uni00D5 | Otilde
102 | Ọ | uni1ECC | Odotbelow
103 | o | uni006F | o
104 | ó | uni00F3 | oacute
105 | ò | uni00F2 | ograve
106 | ỏ | uni1ECF | ohoi
107 | õ | uni00F5 | otilde
108 | ọ | uni1ECD | odotbelow
109 | Ô | uni00D4 | Ocircumflex
110 | Ố | uni1ED0 | Ocircumflexacute
111 | Ồ | uni1ED2 | Ocircumflexgrave
112 | Ổ | uni1ED4 | Ocircumflexhoi
113 | Ỗ | uni1ED6 | Ocircumflextilde
114 | Ộ | uni1ED8 | Ocircumflexdotbelow
115 | ô | uni00F4 | ocircumflex
116 | ố | uni1ED1 | ocircumflexacute
117 | ồ | uni1ED3 | ocircumflexgrave
118 | ổ | uni1ED5 | ocircumflexhoi
119 | ỗ | uni1ED7 | ocircumflextilde
120 | ộ | uni1ED9 | ocircumflexdotbelow
121 | Ơ | uni01A0 | Ohorn
122 | Ớ | uni1EDA | Ohornacute
123 | Ờ | uni1EDC | Ohorngrave
124 | Ở | uni1EDE | Ohornhoi
125 | Ỡ | uni1EE0 | Ohorntilde
126 | Ợ | uni1EE2 | Ohorndotbelow
127 | ơ | uni01A1 | ohorn
128 | ớ | uni1EDB | ohornacute
129 | ờ | uni1EDD | ohorngrave
130 | ở | uni1EDF | ohornhoi
131 | ỡ | uni1EE1 | ohorntilde
132 | ợ | uni1EE3 | ohorndotbelow
133 | U | uni0055 | U
134 | Ú | uni00DA | Uacute
135 | Ù | uni00D9 | Ugrave
136 | Ủ | uni1EE6 | Uhoi
137 | Ũ | uni0168 | Utilde
138 | Ụ | uni1EE4 | Udotbelow
139 | u | uni0075 | u
140 | ú | uni00FA | uacute
141 | ù | uni00F9 | ugrave
142 | ủ | uni1EE7 | uhoi
143 | ũ | uni0169 | utilde
144 | ụ | uni1EE5 | udotbelow
145 | Ư | uni01AF | Uhorn
146 | Ứ | uni1EE8 | Uhornacute
147 | Ừ | uni1EEA | Uhorngrave
148 | Ử | uni1EEC | Uhornhoi
149 | Ữ | uni1EEE | Uhorntilde
150 | Ự | uni1EF0 | Uhorndotbelow
151 | ư | uni01B0 | uhorn
152 | ứ | uni1EE9 | uhornacute
153 | ừ | uni1EEB | uhorngrave
154 | ử | uni1EED | uhornhoi
155 | ữ | uni1EEF | uhorntilde
156 | ự | uni1EF1 | uhorndotbelow
157 | Y | uni0059 | Y
158 | Ý | uni00DD | Yacute
159 | Ỳ | uni1EF2 | Ygrave
160 | Ỷ | uni1EF6 | Yhoi
161 | Ỹ | uni1EF8 | Ytilde
162 | Ỵ | uni1EF4 | Ydotbelow
163 | y | uni0079 | y
164 | ý | uni00FD | yacute
165 | ỳ | uni1EF3 | ygrave
166 | ỷ | uni1EF7 | yhoi
167 | ỹ | uni1EF9 | ytilde
168 | ỵ | uni1EF5 | ydotbelow
169 | D | uni0044 | D
170 | Đ | uni0110 | Dcroat
171 | d | uni0064 | d
172 | đ | uni0111 | dcroat
173 | † | uni2020 | dagger
174 | ‡ | uni2021 | daggerdbl
175 | § | uni00A7 | section
176 | ¶ | uni00B6 | paragraph
177 | ¬ | uni00AC | logicalnot
178 | • | uni2022 | bullet
179 | ◊ | uni25CA | lozenge
180 | ※ | uni203B | referencemark
181 | B | uni0042 | B
182 | C | uni0043 | C
183 | F | uni0046 | F
184 | G | uni0047 | G
185 | H | uni0048 | H
186 | J | uni004A | J
187 | K | uni004B | K
188 | L | uni004C | L
189 | M | uni004D | M
190 | N | uni004E | N
191 | P | uni0050 | P
192 | Q | uni0051 | Q
193 | b | uni0062 | b
194 | c | uni0063 | c
195 | f | uni0066 | f
196 | g | uni0067 | g
197 | h | uni0068 | h
198 | j | uni006A | j
199 | k | uni006B | k
200 | l | uni006C | l
201 | m | uni006D | m
202 | n | uni006E | n
203 | p | uni0070 | p
204 | q | uni0071 | q
205 | R | uni0052 | R
206 | S | uni0053 | S
207 | T | uni0054 | T
208 | V | uni0056 | V
209 | W | uni0057 | W
210 | X | uni0058 | X
211 | Z | uni005A | Z
212 | 1 | uni0031 | one
213 | 2 | uni0032 | two
214 | 3 | uni0033 | three
215 | 4 | uni0034 | four
216 | 5 | uni0035 | five
217 | r | uni0072 | r
218 | s | uni0073 | s
219 | t | uni0074 | t
220 | v | uni0076 | v
221 | w | uni0077 | w
222 | x | uni0078 | x
223 | z | uni007A | z
224 | 6 | uni0036 | six
225 | 7 | uni0037 | seven
226 | 8 | uni0038 | eight
227 | 9 | uni0039 | nine
228 | 0 | uni0030 | zero
229 | \| | uni007C | bar
230 | / | uni002F | slash
231 | \ | uni005C | backslash
232 | @ | uni0040 | at
233 | # | uni0023 | numbersign
234 | & | uni0026 | ampersand
235 | * | uni002A | asterisk
236 | . | uni002E | period
237 | , | uni002C | comma
238 | : | uni003A | colon
239 | ' | uni0027 | quotesingle
240 | “ | uni201C | quotedblleft
241 | ¢ | uni00A2 | cent
242 | £ | uni00A3 | sterling
243 | ¤ | uni00A4 | currency
244 | ¥ | uni00A5 | yen
245 | $ | uni0024 | dollar
246 | € | uni20AC | Euro
247 | ₫ | uni20AB | uni20AB
248 | 。 | uni3002 | ideographicperiod
249 | ， | uniFF0C | commamonospace
250 | ; | uni003B | semicolon
251 | " | uni0022 | quotedbl
252 | ” | uni201D | quotedblright
253 | ( | uni0028 | parenleft
254 | ) | uni0029 | parenright
255 | [ | uni005B | bracketleft
256 | ] | uni005D | bracketright
257 | 〚 | uni301A | whitesquarebracketleft
258 | 〛 | uni301B | whitesquarebracketright
259 | { | uni007B | braceleft
260 | } | uni007D | braceright
261 | ‹ | uni2039 | guilsinglleft
262 | › | uni203A | guilsinglright
263 | « | uni00AB | guillemotleft
264 | » | uni00BB | guillemotright
265 | 〈 | uni3008 | anglebracketleft
266 | 〉 | uni3009 | anglebracketright
267 | 《 | uni300A | dblanglebracketleft
268 | 》 | uni300B | dblanglebracketright
269 | 「 | uni300C | cornerbracketleft
270 | 」 | uni300D | cornerbracketright
271 | 『 | uni300E | whitecornerbracketleft
272 | 』 | uni300F | whitecornerbracketright
273 | 【 | uni3010 | blacklenticularbracketleft
274 | 】 | uni3011 | blacklenticularbracketright
275 | 〖 | uni3016 | whitelenticularbracketleft
276 | 〗 | uni3017 | whitelenticularbracketright
277 | 〔 | uni3014 | tortoiseshellbracketleft
278 | 〕 | uni3015 | tortoiseshellbracketright
279 | 〘 | uni3018 | whitetortoiseshellbracketleft
280 | 〙 | uni3019 | whitetortoiseshellbracketright
281 | + | uni002B | plus
282 | − | uni2212 | minus
283 | × | uni00D7 | multiply
284 | ÷ | uni00F7 | divide
285 | ⁄ | uni2044 | fraction
286 | _ | uni005F | underscore
287 | - | uni002D | hyphen
288 | ± | uni00B1 | plusminus
289 | ︵ | uniFE35 | parenleftvertical
290 | ﹇ | uniFE47 | squarebracketleftvertical
291 | ︷ | uniFE37 | braceleftvertical
292 | ︿ | uniFE3F | anglebracketleftvertical
293 | ︹ | uniFE39 | tortoiseshellbracketleftvertical
294 | < | uni003C | less
295 | = | uni003D | equal
296 | > | uni003E | greater
297 | ~ | uni007E | asciitilde
298 | ! | uni0021 | exclam
299 | ¡ | uni00A1 | exclamdown
300 | ‼ | uni203C | exclamdbl
301 | ︶ | uniFE36 | parenrightvertical
302 | ﹈ | uniFE48 | squarebracketrightvertical
303 | ︸ | uniFE38 | bracerightvertical
304 | ﹀ | uniFE40 | anglebracketrightvertical
305 | ︺ | uniFE3A | tortoiseshellbracketrightvertical
306 | ≤ | uni2264 | lessequal
307 | ≠ | uni2260 | notequal
308 | ≥ | uni2265 | greaterequal
309 | ≈ | uni2248 | approxequal
310 | ? | uni003F | question
311 | ¿ | uni00BF | questiondown
312 | ¦ | uni00A6 | brokenbar
313 | ︽ | uniFE3D | dblanglebracketleftvertical
314 | ﹁ | uniFE41 | cornerbracketleftvertical
315 | ﹃ | uniFE43 | whitecornerbracketleftvertical
316 | ︻ | uniFE3B | blacklenticularbracketleftvertical
317 | ︗ | uniFE17 | bracketwhiteleft-vert
318 | ∫ | uni222B | integral
319 | Ω | uni03A9 | Omega
320 | Δ | uni0394 | Delta
321 | ∏ | uni220F | product
322 | ∑ | uni2211 | summation
323 | ∞ | uni221E | infinity
324 | ^ | uni005E | asciicircum
325 | ︾ | uniFE3E | dblanglebracketrightvertical
326 | ﹂ | uniFE42 | cornerbracketrightvertical
327 | ﹄ | uniFE44 | whitecornerbracketrightvertical
328 | ︼ | uniFE3C | blacklenticularbracketrightvertical
329 | ︘ | uniFE18 | brakcetwhiteright-vert
330 | ∂ | uni2202 | partialdiff
331 | µ | uni00B5 | micro
332 | μ | uni03BC | mu
333 | π | uni03C0 | pi
334 | ƒ | uni0192 | florin
335 | ° | uni00B0 | degree
336 | √ | uni221A | radical
337 | ¹ | uni00B9 | onesuperior
338 | ² | uni00B2 | twosuperior
339 | ³ | uni00B3 | threesuperior
340 | ¼ | uni00BC | onequarter
341 | ½ | uni00BD | onehalf
342 | ¾ | uni00BE | threequarters
343 | % | uni0025 | percent
344 | ‰ | uni2030 | perthousand
345 | ª | uni00AA | ordfeminine
346 | ™ | uni2122 | trademark
347 | © | uni00A9 | copyright
348 | ® | uni00AE | registered
349 | ♥ | uni2665 | heart
350 | ♦ | uni2666 | diamond
351 | ♣ | uni2663 | club
352 | ♠ | uni2660 | spade
353 | ☯ | uni262F | yinyang
354 |  | uniF8FF | apple
355 |  | uniE73A | uniE73A
356 | ︴ | uniFE34 | uniFE34
357 | - | uni00AD | softhyphen
358 | space | uni0020 | space
359 | null | uni0000 | NULL
360 | .notdef |   | .notdef
361 | ☰ | uni2630 | trigramheaven
362 | ☱ | uni2631 | trigramlake
363 | ☲ | uni2632 | trigramfire
364 | ☳ | uni2633 | trigramthunder
365 | ☴ | uni2634 | trigramwind
366 | ☵ | uni2635 | trigramwater
367 | ☶ | uni2636 | trigrammountain
368 | ☷ | uni2637 | trigramearth

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








