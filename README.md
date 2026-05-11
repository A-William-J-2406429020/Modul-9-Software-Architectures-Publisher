1. Step 7\
a. Publisher kamu akan mengirimkan 5 pesan (messages) ke message broker dalam satu kali eksekusi. Hal ini bisa dilihat karena metode p.publish_event() dipanggil tepat lima kali secara berurutan. Setiap panggilan mengirimkan satu objek UserCreatedEventMessage yang berisi data pengguna yang berbeda (Amir, Budi, Cica, Dira, dan Emir).\
b. Publisher maupun subscriber terhubung ke message broker yang persis sama. Dalam sistem antrian pesan (message queuing), broker bertindak sebagai pusat terminal. Agar subscriber berhasil menerima pesan yang dikirim oleh publisher, keduanya wajib terhubung ke alamat server yang sama, di port yang sama, dan menggunakan kredensial yang sama agar bisa saling berkomunikasi di jalur antrean (user_created) tersebut.

2. Running Rabbit MQ:
![](./image/runningrabbit.png)