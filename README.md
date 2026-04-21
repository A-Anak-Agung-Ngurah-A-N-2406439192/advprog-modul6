# advprog-modul6

## Commit 1 Reflection notes

## Commit 1 Reflection notes

Pada commit ini, saya mengimplementasikan *single-threaded web server* dasar menggunakan `TcpListener` untuk mendengarkan koneksi TCP pada `127.0.0.1:7878`. Di dalam fungsi `handle_connection`, setiap request dari *client* (browser) dibaca lebih efisien menggunakan `BufReader` baris demi baris hingga menemukan baris kosong yang menandakan akhir dari HTTP *header*. Setelah itu, seluruh isi request tersebut dikumpulkan dan dicetak ke terminal, sehingga saya bisa melihat secara langsung format request HTTP mentah (seperti *method*, *path*, dan *header*) yang dikirimkan oleh browser. Proses ini memberikan saya pemahaman yang lebih jelas mengenai alur komunikasi awal antara *client* dan *server*.