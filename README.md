Rangkuman OOP
=============

1) apa itu OOP
--------------

object-oriented programming atau OOP adalah suatu metode pemrograman yang lebih berorientasi pada objek.Semua data dan fungsi di dalam metode ini dibungkus dalam kelas atau objek yang nantinya bisa digunakan berulang-ulang dengan cara memanggil kelas dan fungsinya.

2) pembuatan kelas dan objek
----------------------------

pada OOP , kita sering membuat kelas dan objek untuk membungkus suatu data dan fungsi

### objek

Objek merupakan sebuah cara yang digunakan untuk membungkus data dan fungsi menjadi suatu unit dalam sebuah program komputer. Setiap objek memiliki dua karakteristik yaitu Attribute (State) dan Behavior. Attribute (State) merupakan identitas atau informasi objek itu sendiri atau disebut juga sebagai variable, sedangkan Behavior adalah tingkah laku atau apa yang dapat dilakukan oleh objek itu atau disebut juga sebagai method.

contoh:

```
class hewan {       // nama kelas
                public:             // hak akses
                  int kaki;        // Attribute (int variabel)
                  string nama;  // Attribute (string variabel)
              };
              
              int main() {
                hewan myObj;  // membuat objek dengan nama myobj
              
                // mengakses attributes dan menetapkan nilai
                myObj.kaki = 2; 
                myObj.nama = "Ayam";
              
                // cetak nilai attribute
                cout << myObj.kaki << "\n";
                cout << myObj.nama;
                return 0;
              }
```

### Kelas

Class adalah cetak biru (rancangan) atau prototype atau template dari objek. Kita bisa membuat banyak objek dari satu macam class. Class mendefinisikan sebuah tipe dari objek. Di dalam class kita dapat mendeklarasikan variabel dan menciptakan objek (instansiasi). Sebuah class mempunyai anggota yang terdiri dari atribut dan method. Atribut adalah semua field identitas yang kita berikan pada suatu class, misal class manusia memiliki field atribut berupa nama dan umur. Method dapat kita artikan sebagai semua fungsi ataupun prosedur yang merupakan perilaku (behaviour) dari suatu class.

contoh


```
class hewan {       // nama kelas
            public:             // hak akses
              int kaki;        // Attribute (int variabel)
              string nama;  // Attribute (string variabel)
          };
```

3) membuat fungsi pada class
----------------------------

ada 2 cara membuat fungsi pada kelas

A) membuat fungsi didalam kelas

```
 class MyClass {        // nama kelas
            public:              // hak akses
              void myMethod() {  // fungsi dibuat didalam kelas
                cout << "Hello World!";
              }
          };
          
          int main() { 
            MyClass myObj;     // membuat objek dengan nama myObj
            myObj.myMethod();  // memanggil fungsi
            return 0;
          }
```

B) membuat fungsi diluar kelas

```
class MyClass {         // nama kelas 
    public:             // hak akses 
    void myMethod();    // mendeklarasikan fungsi didalam kelas 
    }; 

    // namun isi dari fungsi tersebut dibuat diluar kelas 
    void MyClass::myMethod() {
        cout << "Hello World!"; 
        } 
    
    int main() { 
        MyClass myObj; // membuat objek dengan nama myObj myObj.myMethod(); // memanggil fungsi return 0; 
        }
```

4) penggunaan public, private, protected
----------------------------------------

perbedaan penggunaan public, private, protected terletak pada hak aksesnya

Ketika sebuah property maupun method di set menjadi public, maka seluruh kode program di luar maupun didalam dari class bisa mengakses property maupun method tersebut, termasuk juga untuk class turunannya.

Ketika sebuah property maupun method di set menjadi private, maka yang bisa mengaksesnya adalah hanya class itu sendiri, Dan class lain maupun class turunannya tidak bisa mengakses property atau method tersebut.

Ketika sebuah property maupun method di set menjadi protected, maka yang bisa mengaksesnya adalah class itu sendiri atau turunan dari class tersebut namun tidak bisa diakses dari luar class maupun turunan dari class tersebut.

5) encapsulation
----------------

Encapsulation adalah sebuah konsep Object Oriented Programming digunakan untuk membungkus data dan fungsi, untuk menjaga tetap terjaga agar tidak diakses oleh perintah lain diluar kelas. Untuk bisa mengubah atau mengakses data yang dienkapsulasi perlu membuat fungsi setter dan getter. Konsep encapsulation menyebabkan sebuah konsep OOP yang bernama “Abstraction” atau “Data Hiding”.

contoh

```
class number{ 
    private: 
    int angka; 

    public: 
    void setAngka(int i){ // membuat fungsi setter 
    angka = i; } 
    
    int getAngka(){ // membuat fungsi getter 
    return angka; } 
    }; 

    int main(){ 
    number bilBulat;
    bilBulat.setAngka(0); 
    cout << bilBulat.getAngka() ;
     return 0; 
    }
```

6) inheritance
--------------

Inheritance adalah pewarisan yang artinya sebuah class dapat mewarisi atribut dan method dari class lain. untuk mendeklarasikan suatu class sebagai subclass dilakukan dengan cara menambahkan kata kunci extends setelah deklarasi nama class, kemudian diikuti dengan nama parent class-nya

```
// parent class 
class Vehicle { 
    public: 
    string brand = "Ford"; 
    void honk() {
         cout << "Tuut, tuut! \n" ; } 
         }; 

// child class 
class Car: public Vehicle { 
public: 
string model = "Mustang"; 
}; 
            
int main() {
    Car myCar; 
    myCar.honk(); 
    cout << myCar.brand + " " + myCar.model; r
    eturn 0; 
    }
```# halo
# halo
# halo
# halo
# halo
# halo
# halo
