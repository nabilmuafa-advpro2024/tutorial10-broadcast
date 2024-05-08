# Tutorial 10.2 Reflection Notes

## 2.1 Original code of broadcast chat

![1 server 3 client on tmux](image.png)

Pada gambar ini, kiri atas adalah server sementara yang lainnya adalah client. Untuk menjalankan server ataupun client, perlu dijalankan perintah `cargo run --bin (server/client)`. Jadi dalam kasus ini, saya menjalankan `cargo run --bin server` di kiri atas dan `cargo run --bin client` di instance terminal lainnya. Ketika client dijalankan, maka server akan menangkap bahwa terdapat koneksi baru dari client tersebut, begitu juga dari client-client lainnya. Ketika saya mengetik di salah satu client, maka pesan dari client tersebut akan terkirim ke server, dan kemudian pesan tersebut akan di-broadcast ke server oleh setiap client yang terkoneksi ke server. Itulah mengapa setelah mengetik meskipun hanya di salah satu client, semua client menerima pesan yang diketik.
