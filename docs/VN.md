<p align="center">
  Bản dịch ➜&nbsp;
  <a href="../README.md"><img src="https://flagcdn.com/256x192/us.png" width="48" alt="United States Flag"></a>
  <a href="DE.md"><img src="https://flagcdn.com/256x192/de.png" width="48" alt="Germany Flag"></a>
  <a href="ES.md"><img src="https://flagcdn.com/256x192/es.png" width="48" alt="Spain Flag"></a>
  <a href="FR.md"><img src="https://flagcdn.com/256x192/fr.png" width="48" alt="France Flag"></a>
  <a href="RU.md"><img src="https://flagcdn.com/256x192/ru.png" width="48" alt="Russia Flag"></a>
  <a href="JA.md"><img src="https://flagcdn.com/256x192/jp.png" width="48" alt="Japan Flag"></a>
  <a href="CN.md"><img src="https://flagcdn.com/256x192/cn.png" width="48" alt="China Flag"></a>
  <a href="docs/VN.md"><img src="https://flagcdn.com/256x192/vn.png" width="48" alt="Vietnam Flag"></a>
</p>

---

> [!NOTE] > **Xin chào, sau khi các biện pháp mới được áp dụng tôi đã quyết định phát triển bot này và hoàn thành chỉ trong một ngày. Do các biện pháp này, hiện tại việc làm một bot hoàn toàn tự động có vẻ không khả thi. ~~Tuy nhiên, thông qua một lỗ hổng hiện có chúng ta có thể gửi 12 tài khoản mỗi giây với một lần xác thực, giả sử các tài khoản đầy, 12 \* 62 = <strong>744</strong> pixel/giây.~~ Lỗ hổng này đã được vá sau cập nhật; vì vậy bây giờ bạn sẽ cần lấy token mới cho mỗi lần gửi của mỗi tài khoản. Nếu bạn sẵn sàng, tôi đã mô tả các bước sử dụng bên dưới.**

---

<p align="center"><strong>WPlace UltraBOT</strong></p>

<p align="center">
  Với nhiều tài khoản bạn có thể thêm các pixel bạn muốn vào <a href="https://wplace.live" target="_blank">WPlace</a>.
</p>

---

<p align="center"><strong>🚀┃Cài đặt bot:</strong></p>

<p align="center">
  Việc cài đặt bot dễ, nhưng thành thạo thì khó. Nói đùa thôi, lúc đầu có thể trông khó sử dụng; nhưng với các biện pháp mới được áp dụng không có bot nào khác hoạt động theo cách này. Vì vậy công sức bạn bỏ ra sẽ xứng đáng.
</p>

<br>

### 🔧┃Cài đặt (TR)

- Yêu cầu:

  - Node.js >= 18.18.0

- Các bước:
  1. Cài đặt phụ thuộc:

     ```bash
     npm install
     ```

  2. Khởi động ứng dụng:

     ```bash
     npm start
     ```

  3. Mở `http://localhost:3000` trên trình duyệt.

<details open>
  <summary><h2>📖┃Hướng dẫn</h2></summary>

---

![Phần 1](https://i.imgur.com/yS9093x.png)

Khi truy cập `localhost:3000` bạn sẽ thấy một trang như thế này.<br>

---

![Phần 2](https://i.imgur.com/taF0I2T.png)

Mở một tab mới và vào `chrome://extensions/`.<br>
Bật chế độ nhà phát triển (Developer mode).<br>

![](https://i.imgur.com/oe42A42.png)

Click "Load unpacked".<br>

![](https://i.imgur.com/jPyzOr3.png)

Chọn thư mục `WPlace-Helper`.<br>

---

![Phần 3](https://i.imgur.com/YVyvw3a.png)

Vào trang `wplace.live`.<br>
Nhấn `F12`.<br>
Trong cửa sổ mở ra chọn tab 'Application' ở trên (nếu không thấy hãy bấm vào vùng tôi đánh dấu màu vàng để chọn).<br>
Click vào giá trị `cf_clearance` và copy giá trị bên dưới.<br>

---

![Phần 4](https://i.imgur.com/sJvyiC6.png)

Quay lại bot.<br>
Nhấn nút "Accounts", sau đó nhấn "Add Account". Dán giá trị bạn vừa copy vào ô `cf_clearance`.<br>
Lưu ý!<br>
Vì cập nhật mới có các biện pháp phản phòng, mỗi tài khoản giờ cần một giá trị `cf_clearance` riêng. Để làm nhanh bạn có thể mở wplace.live ở cửa sổ ẩn danh và lấy token. Không cần đăng nhập.

---

![Phần 5](https://i.imgur.com/vJkPMx8.png)

Truy cập `wplace.live` và click vào extension trên thanh trình duyệt, bạn sẽ thấy như hình.<br>
Đảm bảo phần "pixel token" đang bật, sau đó thử vẽ một pixel trên bản đồ bình thường.<br>

![Phần 5 - Lỗi](https://i.imgur.com/uZmJDad.png)

Nếu bạn thấy lỗi này thì bạn đang đi đúng hướng. Click lại extension; thông tin "World X" và "World Y" cho vị trí bạn thử vẽ sẽ hiển thị. Copy chúng.<br>

---

![Phần 6](https://i.imgur.com/LniE1E8.png)

Nhập tọa độ "World X" và "World Y" rồi nhấn 'fetch', bạn sẽ thấy bản đồ như hình.<br>

---

![Phần 7](https://i.imgur.com/vJkPMx8.png)

Quay lại trang trước, click vào extension và copy phần "Account Token".<br>

---

![Phần 8](https://i.imgur.com/8sjhH1L.png)

![Phần 8](https://i.imgur.com/jf6W8NV.png)

Sau đó bạn sẽ được chuyển tới mục Tài khoản. Nhấn "Add Account". Ở trang mở ra:

- Bạn có thể nhập tên bất kỳ cho tài khoản.
- Dán giá trị đã copy vào ô "Account Token".
- Nhấn "Add".<br>

---

![Phần 9](https://i.imgur.com/DJUEywj.png)

Sau khi thêm bao nhiêu tài khoản tùy thích, góc trên bên phải sẽ hiển thị tổng pixel và pixel khả dụng cho tất cả tài khoản.<br>
Hình bạn tải lên sẽ tự động được chuyển sang bảng màu miễn phí có sẵn trên site và được tải lên theo cách đó. Hệ thống này sẽ được cải thiện trong tương lai.<br>

Khi bạn dùng nút "Upload Image":<br>

- Ở góc trên bên trái của hình sẽ hiển thị số pixel cần thiết cho hình.<br>
- Ở góc trên bên phải có nút khóa. Khi khóa, bạn không thể di chuyển hình. Nút 'X' xóa hình.<br>
- Tất cả hình đã tải sẽ hiển thị ở thanh bên trái. Nếu bạn không tìm thấy hình trên trang, click vào thanh để chuyển trực tiếp đến hình đó.<br>

---

![Phần 10](https://i.imgur.com/Dzt1p3o.png)

Nhấn nút "Ready". Trong cửa sổ mở ra nhấn "Select Account" để chọn các tài khoản đang hoạt động. Khi xong nhấn lại "Select Account" để đóng cửa sổ.<br>

---

![Phần 11](https://i.imgur.com/QKJRVL9.png)

Khi zoom vào hình, mỗi pixel trong vùng trong suốt bạn đã tô sẽ được lấp bằng màu tương ứng từ hình tải lên và bạn chỉ có thể đặt pixel trong giới hạn của hình. Nếu chọn một màu cụ thể, bạn có thể vẽ ở bất kỳ vị trí nào miễn là còn trong tổng số pixel tối đa của bạn.<br>

---

![Phần 12](https://i.imgur.com/vJkPMx8.png)

Quay lại trang WPlace và vì token trước đó đã hết hạn, hãy thử gửi một pixel mới; copy giá trị "pixel token" mới.<br>

---

![Phần 13](https://i.imgur.com/wDp07pH.png)

Quay lại trang bot, dán giá trị vào ô 'token' và nhấn 'Start'.<br>

---

![Phần 14](https://i.imgur.com/iQTH5TR.png)

Nếu mọi thứ làm đúng, bạn sẽ nhận được thông báo như hình và thay đổi sẽ được áp dụng trên bản đồ. Vậy là xong; lặp lại các bước này để tạo bất kỳ hình ảnh nào bạn muốn.<br>

</details>

<br>

> [!IMPORTANT]
>
> <p><sub><strong>1.</strong> Trong phần Tài khoản, nếu bạn nhấn 'Check Pixel' bạn có thể kiểm tra thủ công số pixel còn lại cho tài khoản đó. Thông thường hệ thống tự kiểm tra mỗi 90 giây.</sub></p>
> <p><sub><strong>2.</strong> Token tài khoản có hiệu lực khoảng 4-5 giờ. Nếu trong quá trình kiểm tra tự động token hết hạn, tài khoản sẽ chuyển sang trạng thái không hoạt động. Vào phần chỉnh sửa, nhập token mới và nhấn 'Check Pixel' để kích hoạt lại.</sub></p>
> <p><sub><strong>3.</strong> Khi token gửi hiển thị trên bảng, bạn cần nhanh tay. Nếu quá chậm token sẽ hết hạn và bạn sẽ nhận lỗi 403 khi làm mới.</sub></p>

<br>

Toàn bộ dự án được hoàn thành trong 1 ngày, nên đừng quên báo lỗi hoặc tính năng bạn muốn nếu thấy thiếu sót.

---

<p align="center">
  <img src="https://i.imgur.com/msR5dM9.png" alt="Trang Chủ"/>
</p>

---

### 📋┃Danh sách việc cần làm

- [x] Bản dịch [TR/USA]
- [ ] Sửa lỗi script
- [x] Hướng dẫn

---

<p align="center">
  <a href="#"><img src="https://komarev.com/ghpvc/?username=xacter&repo=WPlace-UltraBOT&style=for-the-badge&label=Views:&color=gray"/></a>
</p>
