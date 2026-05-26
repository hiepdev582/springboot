# SpringBoot

## SpringBoot basic

### I. Configuration Classes

1.  Cách nạp thêm các lớp cấu hình khác: Bạn không cần thiết và cũng không nên nhồi nhét tất cả các định nghĩa cấu hình vào một lớp duy nhất. Để chia nhỏ và quản lý, bạn có 2 cách:
    - `@Import`: Dùng chú thích này để chỉ định và nạp trực tiếp các lớp `@Configuration` bổ sung khác vào hệ thống.
    - `@ComponentScan`: Tự động quét và nhặt tất cả các Spring Component, bao gồm cả các lớp được đánh dấu `@Configuration` nằm trong phạm vi quét.

2.  Cách tiêm cấu hình vào ứng dụng
    - `@Value`: Tiêm trực tiếp giá trị của một thuộc tính vào biến.
    - `@ConfigurationProperties`: Ràng buộc cấu hình ngoại ứng dụng vào một đối tượng Java có cấu trúc, giúp quản lý dữ liệu an toàn theo kiểu dữ liệu (Type-safe).
    - `Environment`: Truy xuất thủ công các cấu hình thông qua đối tượng môi trường của Spring.

3.  File cấu hình riêng cho từng Profile
    - `application-{profile}.properties` hoặc `application-{profile}.yaml`
