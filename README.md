# Nindia Nur Artika I.2510256
# JavaPersistence - Employee Management Application

Aplikasi desktop CRUD (Create, Read, Update, Delete) untuk manajemen data karyawan menggunakan **Java 21 LTS**, **Hibernate ORM**, dan **MySQL Database**.

---

# Employee Management App (Java Persistence)

Aplikasi CRUD Desktop berbasis **Java 21**, **Hibernate ORM**, dan **MySQL** untuk manajemen data karyawan.

## 🛠️ Persyaratan Sistem
* **Java JDK 21**
* **Maven 3.9.x**
* **MySQL Server 8.0+**

---

## 🗄️ Database Quick Start

1.  **Buat Database:**
    ```sql
    CREATE DATABASE latihan;
    USE latihan;
    ```
2.  **Struktur Tabel:**
    ```sql
    CREATE TABLE karyawan (
        nip VARCHAR(10) PRIMARY KEY,
        nm_kar VARCHAR(100) NOT NULL,
        tem_lhr VARCHAR(50) NOT NULL,
        tgl_lhr DATE NOT NULL,
        jabatan VARCHAR(50) NOT NULL
    );
    ```

---

## ⚙️ Konfigurasi
Sesuaikan kredensial database pada file:  
`src/main/resources/META-INF/persistence.xml`

```xml
<property name="jakarta.persistence.jdbc.url" value="jdbc:mysql://localhost:3306/latihan"/>
<property name="jakarta.persistence.jdbc.user" value="root"/>
<property name="jakarta.persistence.jdbc.password" value="PASSWORD_ANDA"/>
```

---

## 🚀 Cara Menjalankan

Gunakan perintah terminal berikut:
```bash
# Build proyek
mvn clean compile

# Jalankan aplikasi
mvn exec:java
```

---

## 📂 Struktur Proyek Singkat
* `Karyawan.java`: Model Entity.
* `ControllerKaryawan.java`: Logika akses data (DAO).
* `FormKaryawan.java`: Antarmuka GUI.
* `persistence.xml`: Konfigurasi Hibernate.

---

## 💡 Fitur Utama
* **CRUD Lengkap:** Tambah, Lihat, Ubah, dan Hapus data.
* **Pencarian:** Cari data berdasarkan NIP.
* **Validasi:** Penanganan error input dan duplikasi data.
* **UI Modern:** Menggunakan JSplitPane untuk layout yang rapi.
---

<img width="984" height="640" alt="image" src="https://github.com/user-attachments/assets/84109ed2-4264-47a1-bede-5bb1b11b8548" />

