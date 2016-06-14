---
layout: post
title:  A useful CAPSLOCKS
date:   2016-04-27 11:52:58 +0700
categories: tips
header-img: http://www.howtogeek.com/wp-content/uploads/gg/up/xsshot4d0bb21e1804e.jpg.pagespeed.gp+jp+jw+pj+js+rj+rp+rw+ri+cp+md.ic.0fRzh_qKvO.jpg
---
Mỗi dev, mỗi project ... thì sẽ có những **stack** riêng, [Check MeoBeoI stacks](http://stackshare.io/MeoBeoI), khi làm thi thoảng cũng phải switch qua lại giữa các app ( software ... ), **thao tác** của bạn sẽ làm như thế nào ?

Một cô làm việc trên **Windows** :
+ Click vào icon trên destop
+ Click vào **pined app** ở **Taskbar**
+ **Pin app** vào <strong>taskbar </strong>rồi bấm <kbd><i class="fa fa-windows" aria-hidden="true"></i></kbd> + <kbd>1</kbd> <kbd>2</kbd><kbd>3</kbd> hay <kbd>Alt</kbd> + <kbd>Tab</kbd>

Một chú thao tác trên **MAC** :
+ <kbd>Cmd</kbd> <kbd>Space</kbd> open **Spotlight** => **app name** => <kbd>enter</kbd>

Bạn mình nói :

> Phím CAPS LOCK có bao giờ dùng đâu, chỉ toàn bấm nhầm vào thôi 

![Em nó đây](https://elitekeyboards.com/proddata/images/th/pdkb400b_full1000_th0x0.jpg)

Thấy cũng đúng, **dev lông** thì cần gì **CAPLOCKS**, thế là hành trình biến đổi **CAPLOCKS** bắt đầu từ đây.

<span style="color : red;">macOS only ( help me to bring this to Window, Linux ... )</span>

## Mục tiêu : Mở app nhanh với hotkey

### Step 1 : Tạo service để chạy app
1. Vào **Automator ==> Service**
2. **Launch Application** ( nhớ chọn "no input" như hình nha )
![step1-2](http://i.imgur.com/d3G4qgl.png)
3. Kéo cái **Launch Application** vào chỗ `Drag actions or files here to build your workflow` chứ gì nữa
4. **Chọn Application**, bấm nút ▶️ (RUN) xem có chạy được k nào.
5. Save lại với tên gợi nghĩa ( open Sublime, open Terminal ...)

### Step 2 : Dùng shortcut để chạy service
1. Vào **Keyboard ==> Shortcut ==> Services**
2. Tùy vào trí tưởng tượng hay gì gì đó của bạn mà đặt **Hotkey** vào đó để chạy cái service đó
    - Recommend : <kbd>F19</kbd> + <kbd>A letter</kbd> ( vd: <kbd>F19</kbd> + <kbd>S</kbd> for **S**ublime)  😼
    - WTH is <kbd>F19</kbd> ==> <kbd>F19</kbd> = <kbd>shift</kbd> + <kbd>ctrl</kbd> + <kbd>alt</kbd> + <kbd>⌘</kbd>
![step2-2](http://i.imgur.com/w9zeL6m.png)
3. Giờ thì ra bấm thử **Hotkey đó** xem có mở Sublime hay cái gì gì của chưa nào

Đến đây là cơ bản đã đủ để bạn chuyển App nhờ hotkey rồi, nhưng theo như recommend thì phải bấm **5 nút** để chuyển app thì hơi khó khăn.
Để giải quyết vấn đề trên, Next Step sẽ giúp bạn thay phím <kbd>caps lock</kbd> = <kbd>F19</kbd>


### Step 3 : A useful CAPS LOCK
1. Down và install <a href="https://pqrs.org/osx/karabiner/index.html.en" target="_blank">Karabier</a>
2. **Open Karabier --> Misc & Uninstall --> <kbd>open private.xml</kbd>**
3. Paste của nợ này vào
<script src="https://gist.github.com/MeoBeoI/11ec42dd99ca06d40148.js"></script>
4. **Change Key** --> **Reload XML** --> check **F19 to F19**
5. Down và install <a href="https://pqrs.org/osx/karabiner/seil.html.en" target="_blank">Seil</a> ( đây là utility bổ trợ cho Karabier )
6. Flow these : [Usage of Seil](https://pqrs.org/osx/karabiner/seil.html.en#usage) ( too lazy to copy and paste 😴 )

Xong rồi đó, thử <kbd>caps lock</kbd> + <kbd>X</kbd> xem, Chắc là OK 🌱

#### Lời tựa cuối
Hy vọng thay đổi nhỏ này sẽ giúp bạn có thể tự tin ra lệnh cho máy vi tính của mình, bắt nó làm theo ý muốn, người ngoài nhìn vào thấy hoành tráng, và chính nhất là **Nâng cao hiệu quả công việc**

Vẫn còn một số sạn khi sử dụng cách này, nhưng sạn cũng không to lắm ( 1 số App khi chạy k dùng Hotkey chuyển app khác đc ), nên bạn cứ yên tâm mà dùng.

Đây chỉ áp dụng cho **macOS**, bạn nào dùng **Linux, Window ...** nếu biết cách nào, thì nhanh nhanh tạo [Pull request](https://github.com/codeconcat/codeconcat.github.io/pulls) cho mình nào.


#### Cảm ơn và tham khảo nè:

+ [Google - "a useful caps lock"](https://www.google.com/search?client=safari&amp;rls=en&amp;q=a+useful+caps+lock&amp;ie=UTF-8&amp;oe=UTF-8"target="_blank">)
+ [anh.at](http://anhd.at")

