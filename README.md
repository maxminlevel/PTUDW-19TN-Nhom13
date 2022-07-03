# PTUDW-19TN-NHOM13

## Prototype 1: 
### Convention:
- Nhằm tránh confict css nên chia css ra từng trang riêng, với các style dành cho navbar, sidebar hoặc các component dùng chung thì đưa vào thư mục shared
- Tương tự lý do với html
- Mọi hình ảnh đều đưa vào image
- Với hình ảnh của các món ăn thì cho vào thư mục images/products
- Data dạng json thì cho vào thư mục data
- Đặt tên class theo format [BEM](https://topdev.vn/blog/bem-la-gi/#:~:text=BEM%20l%C3%A0%20vi%E1%BA%BFt%20t%E1%BA%AFt%20c%E1%BB%A7a%20Block-Element-Modifier%2C%20l%C3%A0%20m%E1%BB%99t,ngh%C4%A9a%20g%C3%AC%2C%20n%C3%B3%20th%E1%BB%B1c%20hi%E1%BB%87n%20nhi%E1%BB%87m%20v%E1%BB%A5%20g%C3%AC) trong đó:
  - Ví dụ:
  ```
  Trường hợp các block
  .m__container làm nhiệm vụ cân max width và padding left right
  .m__inner làm nhiệm vụ cân padding top bottom và điểm bám cho các element absolute. VD: chỉnh một button…
  .m__header chứa Sub-title.
  .m__content chứa Headline và Description.
  .m__footer chứa button CTA.
  Trường hợp các element
  .m__headline là Text cỡ lớn. Style thường là H1 hoặc H2.
  .m__intro, .td__description làm mô tả content.
  .m__image chứa ảnh.
  .m__button với style riêng cho button trong section này.
  Trường hợp các modifer
  .m__button--red
  .m__button--active
  ```
  - m là manager
  - c là customer
  - a là admin
  - s là cho component/html/css dùng chung

### Tool:
- Sử dụng jquery để load các component dùng chung thông qua id. Ví dụ: Navbar, sidebar, paging bar, footer
- Sử dụng cli node-sass để compile css:
  ```bash
  npm install
  npm run compile:sass  # node-sass sass/main.scss css/style.css -w
  ```
  File style.css sẽ tự động build khi bạn lưu file scss.

### Deploy:
- Sử dụng netilify
  - Build với lệnh: ```npm instal && node-sass sass/main.scss css/style.css -o```
- Nhánh production: main
- Nhánh preview: develop
- Nhánh còn lại để cài đặt tính năng

## Contributor:
<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://maxminlevel.github.io"><img src="https://avatars.githubusercontent.com/u/23698695?v=4?s=100" width="100px;" alt=""/><br /><sub><b>V.Toan Vo</b></sub></a><br /><a href="" title="Content">🖋</a> <a href="" title="Code">💻</a> <a href="#design-corneliusroemer" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/tnghung"><img src="https://avatars.githubusercontent.com/u/100503370?v=4?s=100" width="100px;" alt=""/><br /><sub><b>N.Hung Trinh</b></sub></a><br /><a href="" title="Technical">📖</a><a href="" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/drwpls"><img src="https://avatars.githubusercontent.com/u/56083989?v=4?s=100" width="100px;" alt=""/><br /><sub><b>L.Son Phan</b></sub></a><br /><a href="" title="Technical">📖</a><a href="" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/NXV5111"><img src="https://avatars.githubusercontent.com/u/66857046?v=4?s=100" width="100px;" alt=""/><br /><sub><b>X.Vy Nguyen</b></sub></a><br /><a href="" title="Technical">📖</a><a href="" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->