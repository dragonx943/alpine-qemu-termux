# alpine-qemu-termux
VIE: Chạy Alpine Linux bằng giả lập QEMU trên Android với Termux!
ENG: Run Alpine Linux on Android with Termux/QEMU!

## How to cài:
Cần: [Termux](https://f-droid.org/repo/com.termux_118.apk), cài `qemu-system-x86_64-headless git wget` thông qua `apt` hoặc `pkg`

Đơn giản thôi:

  ```sh
  git clone https://github.com/dragonx943/alpine-qemu-termux && cd alpine-qemu-termux && chmod a+x vmstart
  ```

  ```sh
  wget https://github.com/dragonx943/alpine-qemu-termux/releases/download/Disk/alpine.qcow2
  ```

  ```sh
  bash vmstart
  ```

Còn lại thì chờ nó chạy và húp thôi. Con máy ghẻ Nokia 6.1 Plus của tôi khởi động Alpine Linux cũng mất gần 2 phút và tắt máy ảo mất mọe 1 phút:(

Nói chung là tùy máy, khỏe thì chạy nhanh, yếu thì đuối vcl không nên thử làm gì. Nếu Android đã Root + Kernel của Android Hỗ trợ KVM thì còn nhanh hơn nhiều...Đã mở cổng 22 trong máy ảo Alpine Linux chính là cổng 2222 của localhost (127.0.0.1 - Android)

==> Chỉ dành cho máy CPU có 8 nhân. Đã tối ưu hóa hệ điều hành Alpine Linux nhờ vài cái forum với ChatGPT, sử dụng ảo hóa TCG + Virtio driver để hi vọng là nó nhanh hơn!

## How to install:
Need: [Termux](https://f-droid.org/repo/com.termux_118.apk), install `qemu-system-x86_64-headless git wget` in Termux using `apt` or `pkg`

Install:

  ```sh
  git clone https://github.com/dragonx943/alpine-qemu-termux && cd alpine-qemu-termux && chmod a+x vmstart
  ```

  ```sh
  wget https://github.com/dragonx943/alpine-qemu-termux/releases/download/Disk/alpine.qcow2
  ```

  ```sh
  bash vmstart
  ```

Boot time / Speed depend on your Android device. If your device is Rooted + Android kernel support KVM, it will be much faster...Opened port 22 in Alpine Linux (VM) = Port 2222 in Android (127.0.0.1 - localhost)

==> Only for Android device have CPU with 8 cores. Optimized Alpine Linux OS by some random forums + ChatGPT, using TCG virtualization + Virtio driver to make VM faster!

## Đóng góp / Contribute
Vui lòng đóng góp bằng cách Folk dự án này về acc GitHub của bạn và sửa đổi, sau đó **Pull Request**

Báo cáo sự cố: [Tại đây](https://github.com/dragonx943/alpine-qemu-termux/issues)
