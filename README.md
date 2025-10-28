# 🌌 Lyra — Music Streaming & Social Listening Platform

> by **Lyra-Net**

> **Nghe nhạc theo cách mới — kết nối, chia sẻ và cảm nhận cùng nhau.**

---

## 🎧 Giới thiệu

**Lyra** là nền tảng **streaming nhạc** hiện đại được phát triển bởi **Lyra-Net**, mang đến trải nghiệm âm nhạc cá nhân hoá và xã hội hoá.  
Với Lyra, người dùng có thể:

- 🎵 **Nghe nhạc trực tuyến** mượt mà, tốc độ cao
- 💿 **Tạo & quản lý playlist cá nhân** dễ dàng
- 📰 **Khám phá feed nhạc & playlist** mới mỗi ngày
- 🤝 **Tham gia phòng nghe chung (Listening Room)** để nghe nhạc đồng bộ với bạn bè
- ❤️ **Tương tác & chia sẻ cảm xúc âm nhạc** trong thời gian thực

Lyra không chỉ là ứng dụng nghe nhạc — mà là **một không gian âm nhạc cộng đồng**, nơi mọi người cùng kết nối thông qua giai điệu.

---

## 🧩 Kiến trúc hệ thống

Lyra được xây dựng theo mô hình **Microservices Architecture**, đảm bảo khả năng mở rộng, dễ bảo trì và hiệu năng cao.

### Các dịch vụ chính:

| Service                  | Mô tả                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------------- |
| **Identity Service**     | Xác thực & quản lý tài khoản người dùng (JWT, session, token rotation, refresh token, v.v.) |
| **Music Service**        | Quản lý metadata của bài hát, album, nghệ sĩ, và playlist                                   |
| **Streaming Service**    | Xử lý & phân phối stream nhạc (Node.js + Kafka)                                             |
| **Feed Service**         | Quản lý feed bài hát/playlist, theo dõi hoạt động của bạn bè                                |
| **Room Service**         | Quản lý Listening Room — đồng bộ playback giữa nhiều client qua WebSocket                   |
| **Notification Service** | Gửi thông báo realtime khi có tương tác mới                                                 |
| **Gateway API**          | Cổng vào hệ thống, hỗ trợ cả gRPC và HTTP (REST) tuỳ theo loại client                       |

---

## 🧠 Công nghệ sử dụng

| Thành phần                 | Công nghệ                                |
| -------------------------- | ---------------------------------------- |
| **Ngôn ngữ chính**         | Go, Node.js, TypeScript                  |
| **Giao tiếp giữa service** | gRPC, Kafka                              |
| **Database**               | PostgreSQL, Redis, MinIO                 |
| **Gateway**                | Apache APISIX                            |
| **Realtime Communication** | WebSocket                                |
| **Triển khai & Scaling**   | Docker, Kubernetes                       |
| **Frontend (Client)**      | React / Next.js (SPA + SSR), TailwindCSS |

---

## 🧭 Định hướng phát triển

- [ ] Tích hợp **AI Recommendation Engine** (gợi ý bài hát theo sở thích)
- [ ] Hỗ trợ **decentralized music ownership** (NFT / on-chain rights)
- [ ] Thêm **voice chat** trong Listening Room
- [ ] Ứng dụng **mobile & desktop app**
- [ ] Hệ thống **token & subscription** cho nghệ sĩ độc lập

## 🤝 Đóng góp

Lyra hoan nghênh mọi đóng góp từ cộng đồng ❤️  
Hãy mở **Pull Request** hoặc **Issue** tại:  
👉 [github.com/Lyra-Net/lyra](https://github.com/Lyra-Net/lyra)

---

## 📜 Giấy phép

Dự án được phát hành dưới giấy phép **MIT License**.  
Xem chi tiết tại [LICENSE](./LICENSE).

---

> “Âm nhạc không chỉ để nghe, mà để **kết nối con người**.  
> Với Lyra, mỗi bài hát là một hành trình — cùng nhau ta tạo nên bản hòa âm bất tận.”
