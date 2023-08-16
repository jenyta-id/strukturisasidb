Database strukturisasi KAMI Foundation menggunakan MySQL

## Proyek apa ini?
Proyek ini adalah implementasi dari struktur basis data untuk mengelola informasi dalam suatu perusahaan, termasuk data departemen, proyek, karyawan, dan hubungan antara karyawan. Basis data ini dibangun menggunakan MySQL dan mengikuti skema Entity-Relationship (ER).

## Skema
Skema basis data yang diimplementasi
- Tabel "departments"
    - [department_id] Primary Key
    - department_name
- Tabel "projects"
    - [project_id] Primary Key
    - project_name
    - start_date
    - end_date
- Tabel "employees"
    - [employee_id] Primary Key
    - first_name
    - last_name
    - birth_date
    - hire_date
    - [department_id] Foreign Key
    - position
- Tabel "employee_projects"
    - [employee_id] Foreign Key
    - [project_id] Foreign Key

## Konsep
`Entitas` &mdash; Tabel "departments", "projects", dan "employees" mewakili entitas dalam lingkungan perusahaan, seperti departemen, proyek, dan karyawan.
`Atribut` &mdash; Setiap kolom dalam tabel mewakili atribut dari entitas, seperti nama departemen, nama proyek, tanggal lahir karyawan, dll.
`Primary Key` &mdash; Setiap tabel memiliki kolom yang berfungsi sebagai primary key, yang unik untuk setiap baris dan digunakan untuk mengidentifikasi entitas.
`Foreign Key` &mdash; Kolom [department_id] dalam tabel "employees" dan kolom [employee_id] serta [project_id] dalam tabel "employee_projects" adalah contoh foreign keys yang menghubungkan entitas di tabel yang berbeda.
`Relasi` &mdash; Hubungan antara entitas diwakili oleh foreign keys. Seperti hubungan antara karyawan dan departemen terjadi melalui [department_id] dalam tabel "employees".

## Penggunaan
Silahkan Clone agar dapat menjalankan skrip ini menggunakan perintah SQL pada server MySQL Anda. Clone disini dimaksudkan untuk menduplikat sebuah repository. Proses clone ini biasanya digunakan oleh para developer untuk berkolaborasi di dalam sebuah project, jadi sebuah project dikerjakan oleh lebih dari 1 orang dan project tersebut disimpan di 1 repository saja.
	$ git clone 

## Visual
<img src="#"/>

Thanks
