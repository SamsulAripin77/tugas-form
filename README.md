# tugas-form

## Part 1 : slicing 
- slicing screenshot page pada gambar menjadi halaman web
- harus menggunakan native php 1 file untuk  1 page
- harus harus bisa mengirim data ke backend ketika mathod submit, boleh disimpan langsung ke db atau disimpan di return balik dalam bentuk aray
- gunakan javascript untuk memanipulasi form yang memliki nested input data ( sub data )
- boleh menggunakan pure css, menggunanak tailwind / css menjadi nilai plus

## Part 2 : membuat dashobard
+ basic
  - convert project slicing sebelumnya ke dalam laravel
  - buat project laravel versi bebas minimal versi 8
  - buat fungsi login register dengan laravel breeze : https://laravel.com/docs/11.x/starter-kits
  - buat dashboard dengan Admin LTE atau optional menggunakan library lain jika menggunakan tailwind : https://adminlte.io/
  - buatkan crud database untuk form2 sebelum nya
  - untuk database wajib dibuat menggunakan migration
  - implementasikan web component pada field-input di form : https://www.youtube.com/watch?v=KVJbzrU6S8E
  - gunakan select2 untuk input type select : https://select2.org/getting-started/basic-usage
  - menambahkan validasi seperti require, unique value pada form
  - menggunakan rich text editor untuk input typ text area : https://quilljs.com/
  - buatkan seeder untuk user ( buat 1 akun admin )
  - buatkan seeder & factory untuk semua form minimal 10 data dummy
  
+ optional ( nilai plus )
  - menggunakan popup pada salah satu crud untuk form create dan edit
  - menggunakan ajax request / rest api untuk proses crud tanpa mereload halaman
  - menambahkan sweet alert untuk notifikasi : https://sweetalert2.github.io/
  - menggunakan library google map untuk input lokasi
  - meenggunakan library js untuk upload image/file : https://pqina.nl/filepond/#examples
 
# Part 3 : Advance
- untuk fungsi controller yang menyimpan data ke beberapa tabel sekaligus gunakan sistem database transaction
- tambahkan pagination di tabel
- tambahkan fitur search by name/title diatas tabel
- tambahkan fiture soft delete untuk semua tabel
- tambahkan kolom crated_by, updated_by, value nya harus otomatis terisi berdasarkan id,user yang sedang login
- di semua tabel tambahkan dropdown untuk merubah urutan default descending by id

# Part 4 : Authentikasi dan authorisasi
- menerapkan sistem authentikasi tidak bisa mengakses dashboard keculasi user yang sudah login
- menginstall laravel permission : https://spatie.be/docs/laravel-permission/v6/introduction
- menerapkan sistem user, role, permission
  - buat menu baru bernama manage users yang berisi submenu : user, role, permission. menu ini hanya bisa dikses admin
  - untuk pembuatan role dan permission harus bisa custom se flexible mungkin.
  - tambahkan permission di semua menu sidbar dan route crud.
  - buat 2 role Admin dan User
  - admin bisa melihat semua menu dan semua data
  - user hanya bisa melihat menu yang yang diizinkan ke role nya dan hanya bisa melihat data yang dia buat
