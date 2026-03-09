HƯỚNG DẪN DÙNG

1) MỞ file index.html

2) TÌM đoạn này:
const GITHUB_CONFIG = {
  owner: "YOUR_GITHUB_USERNAME",
  repo: "YOUR_REPO_NAME",
  branch: "main",
  folders: ["crosshair1", "crosshair2"],
  prettifyNames: true
};

3) SỬA thành GitHub của bạn
Ví dụ:
owner: "tengithubcuaban"
repo: "crosshair-gallery"

4) UP các file lên repo GitHub theo cấu trúc:
- index.html
- crosshair1/
- crosshair2/

5) Bật GitHub Pages cho repo.

CÁCH UPDATE SAU NÀY

Bạn chỉ cần:
- upload thêm file PNG vào crosshair1 hoặc crosshair2
- commit / push

Website sẽ tự đọc danh sách file mới từ GitHub repo và hiển thị thêm.
Không cần chạy Python.
Không cần sửa JSON.

LƯU Ý
- Tên hiển thị hiện tại sẽ bỏ .png và đổi "_" "-" thành dấu cách.
  Ví dụ:
  NS_Amethyst_1.png => NS Amethyst 1
  xmas-THF.png => xmas THF

- Nếu muốn giữ nguyên tên file trừ .png:
  trong GITHUB_CONFIG, đổi prettifyNames: true thành false

- Nếu repo của bạn dùng branch khác, sửa branch tương ứng.

- Nếu muốn thêm thư mục thứ 3:
  folders: ["crosshair1", "crosshair2", "crosshair3"]

- Nếu ảnh mới chưa hiện ngay, chờ GitHub Pages cập nhật thêm một chút rồi tải lại trang.

GỢI Ý
Bạn có thể đổi:
- logo CH
- tiêu đề Crosshair Gallery
- màu giao diện
ngay trong index.html.
