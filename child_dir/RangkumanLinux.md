Rangkuman command linux
=======


1\. pwd
=======

akan memberikan informasi mengenai direktori aktif yang sedang kita akses. Hasil dari command adalah seperti /home/username.

2\. cd
======

Jika direktori yang kita akses saat itu ternyata belum tepat, kita bisa memanfaatkan perintah cd (change directory) untuk mengubah atau membuka direktori tertentu. Contohnya, kita sedang berada di direktori Home dan ingin mengakses folder Downloads. Nah, kita hanya perlu menulis perintah cd Downloads.

3\. mkdir
=========

Perintah mkdir (make directory) berfungsi untuk membuat folder atau direktori baru. Untuk menambah direktori Movies, misalnya, kita bisa menulis mkdir Movies.

4\. rmdir
=========

Jika kita ingin menghapus direktori, kita bisa menggunakan perintah rmdir. Namun perlu diketahui, perintah ini hanya bisa menghapus direktori yang masih kosong. Sebagai alternatif, kita juga bisa menulis rm -r untuk mendapatkan fungsi yang sama seperti rmdir.

5\. rm
======

Sedangkan bagi kita yang ingin menghapus satu file secara khusus, kita bisa menambahkan nama file tersebut setelah perintah rm (contoh: rm filename).

6\. cat
=======

Sebagaimana namanya, perintah cat (concatenate) berfungsi untuk menggabungkan files. Contohnya, tulis cat filename1 filename2>filename3 untuk menggabung filename1 dan filename2, dan menjadikannya sebagai filename3. Di samping itu, cat juga menawarkan beberapa fungsi lain, seperti mengetahui konten suatu file (contoh: cat file.txt) dan membuat file baru (contoh: cat > newfile).



7\. echo
========



Perintah echo menawarkan banyak fungsi, salah satunya adalah untuk memasukkan data (yang biasanya berbentuk teks) ke dalam file. Sebagai contoh, kita ingin menambah teks hello there, welcome! ke file bernama sample.txt. Nah untuk melakukannya, kita bisa menulis echo hello there welcome! >> sample.txt.

8\. ls
======


Bagi kita yang ingin mengetahui konten apa saja yang terdapat dalam working directory atau direktori aktif, kita bisa menggunakan perintah ls. Selain itu, kita juga bisa melihat hidden files dengan perintah ls -a, atau melihat konten di direktori lain dengan menulis nama direktorinya seperti ls /home/username/Documents.

9\. locate
==========

jika lupa atau bingung suatu file tersimpat di directori mana maka bisa menggunakan command locate. Jika kita lupa dengan nama file tersebut, kita bisa menambahkan -i, sehingga perintahnya menjadi locate -i filename. Sedangkan jika nama file yang dic ari lebih dari satu kata, kita perlu menambahkan asterisk (\*) ke dalam perintahnya (contoh: locate -i data\*sekolah).

10\. find
=========

kita juga bisa menggunakan find command untuk menemukan suatu file atau direktori. Bedanya, pencarian dengan perintah ini hanya akan difokuskan ke direktori tertentu. Misalnya kita menulis find /nama direktori/ -name sample.txt, maka pencarian tersebut hanya dilakukan pada direktori home yang dituliskan.

11\. touch
==========

Perintah touch bisa digunakan untuk membuat file baru dengan berbagai jenis format; seperti txt, zip, maupun html. Untuk membuat file dengan format teks di direktori Documents, misalnya, kita dapat menulis perintah touch /home/username/Documents/sample.txt,.

12\. sudo
=========

Singkatan dari SuperUser Do; sudo adalah sebuah perintah dasar Linux yang memungkinkan kita menjalankan berbagai macam tasks yang memerlukan root atau administrative permissions. Contoh perintahnya adalah sudo visudo, yang berfungsi untuk mengedit file konfigurasi atau sudoers.

13\. cp
=======

Perintah cp digunakan untuk menyalin file dari direktori aktif ke direktori lain. Contohnya, kita ingin menyalin sample.txt ke direktori Documents. Nah, kita bisa menulis cp sample.txt /home/username/Documents/.

14\. mv
=======

Di sistem operasi Linux, kita juga dapat memindahkan file ke direktori lain dengan bantuan perintah mv. Sebagai contoh, kita menulis mv sample.txt /home/username/Documents/ untuk memindahkan sample.txt ke direktori Documents. Tidak hanya itu, mv juga bisa dimanfaatkan untuk mengubah nama file. Sebagai contoh, kita ingin mengganti nama file txt kita, maka perintahnya akan menjadi mv oldsample.txt newsample.txt.

15\. chmod
=======
Perintah chmod (change mode) berfungsi untuk mengganti izin akses terhadap suatu file atau direktori. Urutan perintahnya adalah chmod [opsi izin akses] [nama file].
Contohnya seperti chmod 754 filename. 

Adapun 754 dalam kode tersebut bisa dirincikan sebagai berikut:
    7 adalah kombinasi dari 4+2+1; berarti user dapat membaca (angka 4), memodifikasi dan menghapus (angka 2), serta menjalankan/mengeksekusi file tersebut (angka 1). 
    5 merupakan gabungan dari 4+0+1; menandakan bahwa anggota group bisa membaca (4) dan menjalankan/mengeksekusi file (1), tetapi tidak bisa memodifikasi dan menghapusnya (0).
    4 adalah kombinasi dari 4+0+0, yang berarti kalau others hanya bisa membaca (4), namun tidak dapat memodifikasi atau menghapus (0) dan menjalankan file (0).      

16\.  grep
=======
grep merupakan salah satu perintah dasar Linux yang paling sering digunakan. Fungsinya adalah untuk mencari teks atau pattern di dalam suatu file. Pola perintahnya yakni grep [opsi] text/pattern [files]. 
Sebagai contoh, Anda menulis perintah grep -i UNix sample.txt. Artinya, Anda sedang mencari kata UNix dalam file sample.txt.
Adapun opsi -i berarti pencarian tersebut akan menampilkan semua baris yang mengandung kata UNix dengan mode case insensitive— tanpa memperdulikan apakah kata tersebut ditulis dalam huruf besar atau kecil. Sehingga kata UNIX, Unix, atau unix pun nantinya akan ditampilkan dalam hasil pencarian.

17\. man
=======
Linux juga menyediakan man command—sebuah perintah yang akan menampilkan halaman manual berisi instruksi atau deskripsi mengenai command tertentu.
Caranya, cukup tulis perintah man diikuti dengan nama command yang ingin Anda ketahui (contoh: man rmdir).  