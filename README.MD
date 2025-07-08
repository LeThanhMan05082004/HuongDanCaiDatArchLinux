# Hướng dẫn cài đặt Arch Linux
Chào mừng đến với hướng dẫn cài đặt Arch Linux cho người không biết gì
## Bước 1: Chuẩn bị môi trường cần thiết
Các bạn cần tải Virtualbox và file iso của Arch Linux
- [Virtualbox](https://www.virtualbox.org/)
- [Arch Linux](https://archlinux.org/download/)
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
### Thao tác thêm các phân vùng mới  
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/26706b60f6c8c37abc9eb87d460088452634db28/HinhAnh/Hinh11.png)
Ở phân vùng đầu tiên mình chỉ cần 2GB, vì này mình sẽ làm phân vùng cho boot, đổi với Arch Linux thì boot đôi khi chỉ cần 521M là đủ rồi, nhưng mình cho nó dư dư chút cho some nhà some cửa =)))
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/bff006542b029110dea5d07018f8d1c6554f8b04/HinhAnh/Hinh12.png)
Phân vùng thành công sẽ như vậy nè
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/fc44218c2c513e0f8d39c33388b65d17e4b07381/HinhAnh/Hinh13.png)
### Thao tác xóa các phân vùng do thêm ngu hoặc thêm lộn =))  
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/0e7a00c95f88db41b4228f95ffdfa988d4f5eb9a/HinhAnh/Hinh14.png)
### Thao tác định dạng phân vùng sẽ thuộc loại gì (không phải định dạng phân vùng, kiểu như là nó sẽ thuộc loại gì để chút định dạng cho dễ, ví dụ loại `linux filesystem` thì là thuộc kiểu dành cho hệ thống, có thể định dạng phân vùng đó dành cho hệ thống, chút nữa làm đến đó sẽ hiểu)  
Mình thì chỉ phân vùng ổ đĩa thành 2 vùng thôi, 1 vùng là cho boot, 1 vùng là cho root, thông thường phải có thêm 1 phân vùng nữa là phân vùng swap, phân vùng swap có chức năng là lấy dung lượng của phần swap ấy, bù cho phần ram của hệ thống bị thiếu khi thực hiện các tác vụ hoặc chạy chương trình.
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/b6e3da33465dd13dea632416c8976897b24c0cbb/HinhAnh/Hinh15.png)
Sau đây mình đã chọn loại cho 2 phân vùng boot và root, hiện tại các bạn không cần biết nó là gì đâu, chỉ cần chọn giống mình là được
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/e5a76d475bfe13bdfbf587514d136780f9d34689/HinhAnh/Hinh16.png)
### Chọn write để lưu lại các phân vùng
![image alt](https://github.com/LeThanhMan05082004/HuongDanCaiDatArchLinux/blob/29966166b6760b87fe1dc657520294d9cf0e80ce/HinhAnh/Hinh17.png)
