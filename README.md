# simple-mvc

Ini adalah contoh implementasi aplikasi **Native PHP** dengan pola **MVC (Model-View-Controller)** yang paling sederhana namun rapi, menggunakan database **MySQL**.

Aplikasi ini akan mengelola data sederhana: **Users** (Nama dan Email).

Ada dua fitur utama:

1.  **Validasi (Server-Side):** Mencegah input kosong atau format email yang salah di _Controller_.
2.  **Bootstrap 5:** Mempercantik tampilan tabel, form, dan tombol di _View_.

Jalankan query SQL ini di pgAdmin atau terminal MySQL Anda untuk membuat tabel:

    CREATE TABLE users (
        id SERIAL PRIMARY KEY,
        name VARCHAR(100) NOT NULL,
        email VARCHAR(100) NOT NULL UNIQUE
    );

    INSERT INTO users (name, email) VALUES ('Budi', 'budi@example.com');
