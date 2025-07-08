# Hướng dẫn cài đặt Arch Linux
Chào mừng đến với hướng dẫn cài đặt Arch Linux cho người không biết gì
## Bước 1: Chuẩn bị môi trường cần thiết
Các bạn cần tải Virtualbox và file iso của Arch Linux
- [ Virtualbox ] : https://www.virtualbox.org/
- [ Arch Linux ] : https://archlinux.org/download/
## Bước 2: Thiết lập môi trường máy ảo
Các bạn vào Virtualbox và bấm vào cái hình màu xanh lam nhạt "New" để tạo máy ảo mới, ở đây là tạo máy ảo Arch Linux
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/9c9107c5c14e7a5477b5021f8de3791b733fb56d/HinhAnh/Hinh1.png)
Nó sẽ ra như thế này ( này là của mình, các bạn có thể đặt tên tùy theo các bạn )
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/c107be81cf98223b1715a164386a5d6825bc6781/HinhAnh/Hinh2.png)
Các bạn bỏ qua phần ở giữa, chuyển qua phần số 3
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/f432fd7de0dee12329eb66e576e5d0f7d2f03c54/HinhAnh/Hinh3.png)
Các bạn sang đến phần cuối cùng, phần này là phần chọn dung lượng cho ỗ đĩa ảo của máy ảo, các bạn để bao nhiêu cũng được, mình thì để tầm 20GB là ổn.
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/c3059c5ff68557ce0b95e5f0af588eb505250a90/HinhAnh/Hinh4.png)
Đã thiết lập xong máy ảo, bấm nút start để chạy máy ảo
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/e2d4e07426ac9d4206d0015edbe150c1439ca643/HinhAnh/Hinh5.png)
## Bước 3: Tiến hành cài đặt Arch Linux
Đây là lần đầu tiên chúng ta khởi động hệ điều hành lên, đây là giao diện mặc định của hệ diều hành, chúng ta sẽ tiến hành cài đặt nó bằng những câu lệnh, không có GUI cài đặt đâu nhé =))
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/99b75db8dd842ce59d029731bd0c1de8d37e6903/HinhAnh/Hinh6.png)
Dùng câu lệnh `setfont ter-132b` để font chữ to hơn để dễ dàng cài đặt
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/e6268b12fb9cb23e3313e1a23c6e82ccb7ef4452/HinhAnh/Hinh7.png)
Phân vùng ổ đĩa, dùng câu lệnh `cfdisk` Chúng ta sẽ chọn GPT để làm dạng chính cho phân vùng ổ đĩa của chúng ta, mình thấy nó tên gpt nên mình lên tưởng đến chat gpt nên mình chọn nó, chứ mình không biết gì hết á, hẹ hẹ hẹ =))
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/f9110729f46b5e4a8b9ca0521db5cafb1fc6f9b9/HinhAnh/Hinh8.png)
Đây là giao diện chính của phân vùng ổ đĩa nè, các bạn không cần biết nhiều đâu, để mình chỉ các bạn vài thao tác cơ bản để phân vùng ổ đĩa
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/bc5ed874036615da8ed59cc80c769886a3c15fb5/HinhAnh/Hinh9.png)
Nhìn xuống dưới, đừng hoảng loạn =)))
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/6bf611caaabd915c99866d892a12f81aca1abfd4/HinhAnh/Hinh10.png)
`New` là nút để tạo phân vùng mới cho ổ đĩa từ cái ổ đĩa chính `FreeSpace`
`Quit` là thoát khỏi chương trình phân vùng ổ đĩa
`Help` là trợ giúp phân vùng ổ đĩa như thế nào, hướng dẫn phân vùng ra sao
`Write` là lưu lại các hoạt động phân vùng, nó sẽ hỏi và yêu cầu nhập `yes` để chấp nhận, chút sẽ thấy
`Dump` cái này không cần biết là gì đâu =)) đừng hỏi GPT nó nói cũng không hiểu đâu =)))
Sau đây là một vài thao tác để tương tác với cái ổ đĩa
- 1. Thao tác thêm các phân vùng mới
- 2. Thao tác xóa các phân vùng do thêm ngu hoặc thêm lộn =))
- 3. Thao tác định dạng phân vùng sẽ thuộc loại gì (không phải định dạng phân vùng, kiểu như là nó sẽ thuộc loại gì để chút định dạng cho dễ, ví dụ loại `linux system` thì là thuộc kiểu dành cho hệ thống, có thể định dạng phân vùng đó dành cho hệ thống, chút nữa làm đến đó sẽ hiểu)

