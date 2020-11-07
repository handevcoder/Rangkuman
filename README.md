># Materials 
## Git Introduction
<div style = "text-align:justify">
Git adalah vesion kontrol system yang digunakan oleh team developer dalam skala yang besar atau kecil. Setiap operasi tersedia secara lokal tanpa koneksi internet yaitu akan di check ketika online.

## Git Basics
### Repo git
Mendapatkan repository git di dalam project, bisa dengan menggunakan dua cara:
1. $ git init untuk menginisialisasi repository git pada project, kemudian akan membuat folder `.git` yang berisikan semua file repository yang akan dibutuhkan git.
2. $ git clone https://github.com/### untuk menduplikasi repository yang sudah ada, pada perintah tersebut akan menduplikasi project sesuai dengan namanya dan di dalam project tersebut sudah terdapat folder `.git`.

### Menyimpan Ke GIT

1. $ git status untuk melihat adakah perubahan pada work directory dan file yang berada di untracked dan tracked.
2. $ git add <file> untuk mengubah status file / direktori menjadi staged.
Mengabaikan file atau direktori bilamana terdapat perubahan di dalamnya, buat file dengan nama `.gitignore` sebagai contoh tambahkan `*.log` dan `build/` untuk mengabaikan perubahan pada file dengan ekstensi log dan folder dengan nama build (termasuk didalamnya).
3. $ git commit -m “message” untuk memasukkan data snapshot ke dalam database git, ubah `message` dengan pesan sesuai kebutuhan, sebagai contoh `initial commit`.

### Menyimpan Perubahan

Selama proses pengerjaan project mungkin ada keinginan untuk mengulangi perubahan file yang sudah di commit atau yang belum di commit, ada beberapa cara untuk mengulangi perubahan tersebut.
1. $ git commit --amend -m “message” untuk melakukan perubahan commit dan nama pesan.
2. $ git reset HEAD `filename` untuk menyetel ulang file tersebut (kembali ke untracked).
3. $ git checkout -- `filename` untuk menyetel ulang file pada commit sebelumnya.

## Git Branch
### Basic Branching

1. $ git branch dev untuk membuat branch dev dan $ git checkout dev untuk berpindah ke branch dev atau dipersingkat dengan $ git checkout -b dev.
2. $ git merge hotfix untuk menggabungkan branch sekarang dengan branch hotfix.
3. $ git branch -d dev untuk menghapus branch dev di lokal.
4. $ git push origin --all untuk berbagi semua branch yang ada di lokal ke remote (biasanya dipakai waktu initial push ke remote).
### Remote Branch
Remote branch merupakan branch yang sudah di kirim ke remote yang berarti orang lain dapat berkontribusi di dalamnya (jika memiliki akses). Langkah yang sering digunakan oleh developer dalam berhubungan dengan remote branch:
1. $ git fetch origin untuk mendapatkan informasi terbaru yang ada di remote dan kemudian $ git merge origin/master untuk menggabungkan informasi tersebut ke local work directory.
2. $ git push origin testing untuk mengirim local branch testing ke remote branch testing (local branch tidak sama dengan remote branch).
3. $ git checkout -b dev origin/dev untuk membuat branch baru dengan titik awal pada remote branch dev.
4. $ git push origin --delete hotfix-auth untuk menghapus remote branch hotfix-auth.

## SDLC dan Figma Introduction
### SDLC
Software Development Life Cycle merupakan sebuah proses yang digunakan oleh industri software untuk mendesign, mengembangkan dan menguji aplikasi dengan kualitas yang tinggi. SDLC memiliki tujuan untuk memproduksi sebuah aplikasi yang memiliki kualitas tinggi sesuai dengan ekspektasi dari customer.

### Tahapan pengembangan pada metode SDLC 
> Planning -> Defining -> Designing -> Building -> Testing -> Deployment -> Maintenance
## Release Planning
Planning atau requirement analysis merupakan tahapan yang penting dalam fundamental SDLC.

### Requirement analysis
Yaitu merencanakan input atau kebutuhan dari customer. Planning juga menjadi tempat untuk melakukan kebutuhan untuk quality assurance dan identifikasi resiko dalam sebuah pengembangan aplikasi.
### Sprint Management

### Defining requirements
Defining requirement merupakan tahapan yang mendefinisikan secara detail mengenai input dari customer. Memberikan gambaran output sebuah dokumen yang isinya seluruh kebutuhan produk yang akan didesain dan dikembangkan.
### Figma

Figma merupakan editor grafis vektor dan alat prototyping berbasis web dan bersifat free.

>#  Kotlin Basic

## Number
 Kotlin yang menyediakan tipe data yang merepresentasikan nilai angka, baik angka bulat maupun angka desimal yaitu number.
2. Byte yang menampung nilai dari -128 sampai 127.
3. Short yang menampung nilai dari -32,768 sampai 32,767.
4. Int yang menampung nilai dari -2,147,483,648 sampai 2,147,> 483,647.
5. Long yang menampung nilai dari -9,223,372,036,854,775,808 sampai 9,223,372,036,854,775,807.

## Operation
>Kotlin mendukung proses aritmatika menggunakan operator ( + ), ( - ), ( / ), ( * ) dan ( % ).
## Strings
>Kotlin menyediakan tipe data text yang berisikan sejumlah
## Angka genap
1. karakter.
2. String
3. Charsequence

> 
##  Angka Desimal
>float yang menampung nilai dari -2,147,483,648.0 sampai 2,147,483,647.0.
>/2. Double yang menampung nilai dari -9,223,372,036,854,775,808. 0 sampai 9,223,372,036,854,775,807.0.

## Booleans
>Kotlin menyediakan tipe data yang hanya memiliki value true atau false yang dinamai dengan Boolean.
Boolean bisa didapatkan dengan kombinasi || atau or, && atau and dan ! (negasi).
## Array
>Arrays di dalam kotlin digunakan untuk menampung data array.
## List
>List merupakan tipe data collection yang sering dipakai di dalam kotlin, ada dua macam list yaitu list (read only) dan mutable list.

# Control Flow
## If Expressions
>Di dalam kotlin if digunakan untuk control flow statement, termasuk dalam konteks ternary operator.

## When Expressions
>When di dalam kotlin merupakan pengganti switch case statement dan penggunaannya lebih simple dibandingkan dengan switch case di bahasa lain.
## For loops
>For di dalam kotlin digunakan untuk melakukan perulangan pada sebuah data collection seperti halnya for di bahasa lain.
```Kotlin var x = (1..100).random()
while (x > 0) {
   println("X: $x")
   x--
}
do {
   val y = (1..3).random()
   println("Y: $y")
} while (y != 1)


````

</div>