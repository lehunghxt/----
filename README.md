#Github
<hr>
##1. Cách thức hoạt động của Github
<img src="https://miro.medium.com/max/700/0*j1QfxoExS1X67_AN.png" alt="">
<p>Mô hình hoạt động của GIT cần nắm một số khái niệm</p>
- Repository (repo): là nơi chứa source code.
- Remote: server online.
- Local: server local trên máy.
- Working copy: nơi làm việc trực tiếp trên máy local.
<p>Chúng ta quản lý source code trên máy sẽ được lưu trữ trên local repo. Khi có internet chúng ta có thể đồng bộ local repo lên online, tức là sync lên remote repo.</p>
<p>Khi trong team hoan thành các tính năng và đã sync lên trên serce online ( remote repo ) thông qua các thao tác ( commit push)</p>

## 2. Các khái niệm cơ bản
- Commit: Lưu các thay đổi từ thư mục đang làm việc (working copy) vào server online (remote repo)
- Push: Cập nhập các thay đổi từ server local ở máy (local repo) lên server online (remote repo).
- Fetch: Để “đồng bộ” mọi thứ thay đổi mới nhất từ server online (remote repo) về server local (local repo) chúng ta sử dụng lệnh fetch ( git fetch)
- Pull: Sau đó để “áp dụng” các thay đổi đó vào source code đang sử dụng.tức là cập nhật từ server local (local repo) vào thư mục đang làm việc (working copy) (git pull)
- Lệnh git clone được dùng với mục đích check out. Nếu respository phụ thuộc vào server từ xa, sử dụng:\ `git clone alex@93.188.160.58:/path/to/repository`
- Add : Lệnh git add có thể được dùng để thêm file vào index. Ví dụ, command sau có thể thêm một file có tên temp.txt vào thư mục local vào index:`git add temp.txt`
- Remove: Xóa tập tin. Bạn có thể xóa bất kỳ tệp nào trong kho của bạn trên GitHub. 
- Fork:  là một bản sao của một kho lưu trữ. `Fork` kho lưu trữ cho phép bạn tự do thử nghiệm các thay đổi mà không ảnh hưởng đến dự án ban đầu. Thông thường nhất, `fork` được sử dụng để đề xuất thay đổi cho dự án của người khác hoặc sử dụng dự án của người khác làm điểm khởi đầu cho ý tưởng của riêng bạn.
- Star: Người dùng trên trang web GitHub có thể "đánh dấu" kho lưu trữ của người khác, do đó lưu họ vào danh sách Repos Starred của họ. Một số người sử dụng "ngôi sao" để chỉ ra rằng họ thích một dự án, những người khác sử dụng chúng làm dấu trang để họ có thể theo dõi những gì đang diễn ra với repo sau này.
- Watch: GitHub luôn giúp bạn dễ dàng "xem" một dự án, điều đó có nghĩa là bạn được thông báo mỗi khi có bất kỳ cập nhật nào.
- 
## 3. Setting up Git
<a href="https://git-scm.com/downloads">Download tại đây.</a>
### 3.1 Download và cài đặt Git

### 3.2 Thiết lập Username của bạn trên Git
<p>Thiết lập username</p>

`$ git config --global user.name "lehunghxt"`

### 3.3 Thiết lập commit email address trên Git

`$ git config --global user.email "leehxt@gmail.com"`

## 4. Generating a new SSH key and adding it to the ssh-agent

### 4.1 Generating a new SSH key
- Mở Git Bash
- Chạy command `$ ssh-keygen -t rsa -b 4096 -C "leehxt@gmail.com"`
- Copy `KEY` trong thư mục /c/Users/you/.ssh/id_rsa.
- Vào <a href="https://github.com/settings/ssh/new">đường dẫn</a> và tạo mới ssh key và paster mã vừa copy vào.

## 5. Caching your GitHub password in Git

Lưu thông tin đăng nhập bằng lệnh: `git config --global credential.helper wincred`.

## 6. Một số lệnh git cơ bản.

### Tạo một kho chứ git: `git init`

### Sao chép một kho chứa git đã tồn tại. `$ git clone https://github.com/user/repository.git`

### Nhánh trong Git

<p>Kiểm tra branch hiện tại</p> 
`$ git branch`
<p>Tạo mới một branch</p>
` $ git branch <name_branch>`
<p>Để chuyển và tạo mới</p>
`$ git branch -b <name_branch>`

### Cập nhập thay đổi

<p>Cập nhập tất cả các file</p>
`$ git add .`
<p>Thay đổi thông tin trên Local Repo</p>
`$ git commit -m "Message"`

### Cập nhập lên Server

<p>Cập nhập lên server thì thực hiện câu lệnh</p>
`$ git push origin <name_branch>`
<p>Nếu chưa tồn tại remote trên server thì bạn cần add mới một remote trước rồi mới push</p>
`$ git remote add origin <remote_url>`
`$ git push origin <name_branch>`

### Xem lại lịch sử commit

`$ git log`







#Markdown

# 2.Markdown là gì?

Markdown là một ngôn ngữ đánh đấu với cú pháp văn bản thô, được thiết kế để có thể dễ dàng chuyển thành HTML và nhiều định dạng khác sử dụng cùng tên. Nó thường được dùng để tạo các tập tin readne, viết tin nhắn trên các diễn đàn, và tạo văn bản có định dạng bằng một trình biên tập văn bản thô.

Năm 2004, cùng với sự giúp đỡ của Aaron Swaetz, John Gruber đã tạo ra ngôn ngữ Markdown với mục tiêu tạo ra một định dạng văn bản thô dễ viết, dễ đọc, dễ dàng chuyển thành HTML hoặc XHTML.

# 3.Tính năng.

**Markdown** dùng các dấu hiệu từ các qui ước văn bản thô trong email, như `settext`- một ngôn ngữ được thiết kế để có thể đọc bình thường mà không phải lục lọi giữ các thẻ định dạng, khác với văn bản trong ngôn ngữ đánh dấu như RTF hay HTML, vốn chứa nhiều thẻ và cú pháp khó đọc. Gruber đã viết một công cụ nhỏ bằng Perl, *Markdown.pl*, cho phép chuyển đổi đoạn văn bản đã đánh dấu theo chuẩn arkdown sang XHTML hoặc HTML. Tiện ích này có thể dùng một mình hoắc dùng như là plugin cho Bloxom hoặc Movable Type, hoặc là một bộ lọc cho BBEdit.

**Markdown** sau đó đã được hoàn thiện thành một mô đun Perl và công bố trên CPAN(Text::Markdown) cũng như trê mottj vài ngô ngữ khác. Nó được phân phối theo giấy phép BSD và được nhúng sẵn, hoặc plugin của một hề thống quản lý nội dung... Một số trang web như Github,reddit,Diaspora, Stack Exchange, OpenStreetMap, SourceForge cũng sử dụng các biến thể của Markdown trong hệ thống của mình.

# 3.1.Thẻ tiêu đề

Tiêu đề được sử đụng bằng cách sử dụng # trước tiêu đề. Số lượng # trước văn bản tiêu đề xác định độ sâu của tiêu đề. Độ sâu của tiêu đề tư 1-6.

**Ví dụ**
```
# Thẻ tiêu đề cấp 1 :thẻ tiêu đề cấp 1.

## Thẻ tiêu đề cấp 2: thẻ tiêu đề cấp 2.

### Thẻ tiêu đề cấp 3: thẻ tiêu đề cấp 3.

#### Thẻ tiêu đề cấp 4: thẻ tiêu đề cấp 4.

##### Thẻ tiêu đề cấp 5: thẻ tiêu đề cấp 5.

###### Thẻ tiêu đề cấp 6: thẻ tiêu đề cấp 6.
```

**Kết quả**


# Thẻ tiêu đề cấp 1 :thẻ tiêu đề cấp 1.

## Thẻ tiêu đề cấp 2: thẻ tiêu đề cấp 2.

### Thẻ tiêu đề cấp 3: thẻ tiêu đề cấp 3.

#### Thẻ tiêu đề cấp 4: thẻ tiêu đề cấp 4.

##### Thẻ tiêu đề cấp 5: thẻ tiêu đề cấp 5.

###### Thẻ tiêu đề cấp 6: thẻ tiêu đề cấp 6.


# 3.2.Chèn link, chèn ảnh.

-Để chèn hyperlink bạn chỉ cần paster link vào file .md .

`http://github.com`

**Kết quả**

http://github.com

Hoặc bạn cũng có thể sử dụng cú pháp sau để thu ngắn đường dẫn của link.


`[Github](https://github.com)`

**Kết quả**

[Github](http://github.com)


-Để chèn ảnh thì bạn sử dụng cú pháp sau:


`<img src="link_anh_cua_ban">`

Ta thường dùng công cụ Snipping Tool có sẵn trên Window để chụp màn hình và up ảnh lên trang http://i.imgur.com/ để lấy đường dẫn ảnh đưa vào Github.
**Ví dụ**


`<img src="http://imgur.com/a/ThgNB">`

**Kết quả:**

<img src="http://i.imgur.com/0x0U3Qx.jpg">

# 3.3.Ký tự in đậm, in nghiêng.

-Để làm đậm một đoạn text, bạn chỉ cần làm như sau:


`**Từ cần in đậm**`

**Kết quả**

**Từ cần in đậm**

-Để in nghiêng một đoạn text bạn chỉ cần làm như sau:


`*Từ cần in nghiêng*`

**Kết quả:** *từ cần in nghiêng*

# 3.4.Trích dẫn bo chữ

-Để bo một đoạn text bạn sử dụng cú pháp sau:


``chữ cần bo``


**Kết quả**


`chữ cần bo`

-Để làm nổi bật một đoạn văn bản, chẳng hạn như một đoạn code bạn có thể sử dụng cú pháp như sau:

```
```sh
#include<stdio.h>
#include<conio.h>
int main()
{
    printf("Hello world.\n");
    getch();
}
```

**Kết quả:**

```sh
#include<stdio.h>
#include<conio.h>
int main()
{
    printf("Hello world.\n");
    getch();
}
```

# 3.5.Gạch đầu dòng

-Để sử dụng gạch đầu dòng, bạn sử dụng cú pháp như sau:

```
-Gạch đầu đong thứ nhất:
<ul>
<li> Thụt đầu dòng 1</li>
<li> Thụt đầu dòng 1</li>
</ul>
-Gạch đầu dòng thứ hai:
<ul>
<li> Thụt đầu dòng 2</li>
<li> Thụt đầu dòng 2</li>
</ul>
```

**Kết quả:**

<ul>
<li> Thụt đầu dòng 1</li>
<li> Thụt đầu dong 2</li>
</ul>
-Gạch đầu dòng thứ hai:
<ul>
<li> Thụt đầu dòng 2</li>
<li> Thụt đầu dòng 2</li>
</ul>

# 3.6.Tạo bảng

-Bạn có thể sử dụng cú pháp sau để tạo bảng:

```
| Cột 1 Hàng 1 | Cột 2 | Cột 3 | Cột 4|
|--------------|-------|-------|------|
|Hàng 2|  2x1  |  2x2  |  2x3  |  2x4 |
|Hàng 3| 3 x 1 | 3 x 2 | 3 x 3 |3 x 4 |
|Hàng 4| 4 x 1 | 4 x 2 | 4 x 3 |4 x 4 |
```

**Kết quả**

| Cột 1 Hàng 1 | Cột 2 | Cột 3 | Cột 4|
|--------------|-------|-------|------|
|Hàng 2|    1  |   4   |   9   |  10  |
|Hàng 3|    2  |   5   |   8   |  11  |
|Hàng 4|    3  |   6   |   7   |  12  |

# 3.7.Tạo chú thích cuối trang



```
-[^1]: chú thích 1.
-[^2]: chú thích 2.
```
>-----------------------------

**Kết quả**

[^1] Chú thích 1.

[^2] Chú thích 2.