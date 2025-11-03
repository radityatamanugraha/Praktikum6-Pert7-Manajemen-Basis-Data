# Tugas Praktikum 6 (Pertemuan ke 7) <img src=https://qph.fs.quoracdn.net/main-qimg-648763cc041459725b62108f4fdf5b91 width="110px">

## Tabel: Tamu
|Nama Atribut|Tipe Data|Keterangan|
|----|---|-----|
|**id_tamu**|**INT (PK)**|**ID unik tamu**|
|**nama_tamu**|**VARCHAR(100)**|**Nama lengkap tamu**|
|**no_telepon**|**VARCHAR(20)**|**Nomor kontak**|
|**email**|**VARCHAR(100)**|**Email tamu**|
|**alamat**|**TEXT**|**Alamat lengkap**|
|**tanggal_daftar**|**DATE**|**Tanggal pertama kali menginap**|

## Tabel: Kamar
|Nama Atribut|Tipe Data|Keterangan|
|----|---|-----|
|**id_kamar**|**INT (PK)**|**ID unik kamar**|
|**nomor_kamar**|**VARCHAR(100)**|**Nomor kamar**|
|**tipe_kamar**|**VARCHAR(50)**|**Tipe (Standard, Deluxe, Suite, dsb)**|
|**status**|**ENUM('Occupied','Vacant','Dirty','Clean','Maintenance')**|**Status kamar**|
|**harga_per_malam**|**DECIMAL(10,2)**|**Tarif per malam**|

## Tabel: Reservasi
|Nama Atribut|Tipe Data|Keterangan|
|----|---|-----|
|**id_reservasi**|**INT (PK)**|**ID unik reservasi**|
|**id_tamu**|**INT (FK)**|**Relasi ke tamu**|
|**tanggal_checkin**|**DATE**|**Tanggal masuk**|
|**tanggal_checkout**|**DATE**|**Tanggal keluar**|
|**status_reservasi**|**ENUM('Booked','CheckedIn','CheckedOut','Cancelled')**|**Status reservasi**|
|**total_biaya**|**DECIMAL(10,2)**|**Total biaya keseluruhan**|












































