# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Herdin Kristianjani Zebua
<br>NIM		        : 1227050053
<br>Jurusan	    	:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks. Dalam matematika, matriks terdiri dari kolom dan baris. Kembali, untuk menentukan nilai dari sebuah matriks, kita harus sebut secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi. Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel,

seperti contoh berikut:
int arr[2][2];

Untuk UAS kali ini membuat 2 buah program yaitu program pertama adalah membuat array 2 dimensi dengan baris , kolom dan nilai nya di input lalu ditukarkan antara kolom dan baris sedangkan program ke dua digunakan untuk mencari nilai yang dapat di bagi 3, 7, dan 5.

Berikut adalah penjelasan source code program yang pertama:

<br>Baris 6 : mendeklarasikan variable i, j, m, n, matriks[10][10], transpose[10][10] dimana variable i digunakan untuk perulangan baris, variable j untuk perulangan  kolom, variable m untuk jumlah baris matriks, variable n untuk jumlah kolom matriks, sedangkan variable matriks[10][10], transpose[10][10] merupakan array dua dimensi yang memiliki maksimal panjang atau ukurun array baris dan kolom sebanyak 10.
<br>baris 8 – 11 : menginputkan nilai ke dalam variable m dan n.
<br>baris 13 – 18 : melakukakan perulangan m (baris) dan n (kolom) untuk menginputkan elemen matriks di variable matriks
<br>baris 20 – 24 : melakukakan perulangan m (baris) dan n (kolom) untuk mengisikan variable transpose matriks dari variable matriks
<br>baris 26 – 32 : melakukakan perulangan n (kolom) dan m (baris) untuk menampilkan hasil operasi tranpose matriks.

<br>Untuk program yang kedua itu kurang lebih sama, hanya berbeda pada perintah hasil output nya saja yaitu menampilkan bilangan yang habis dibagi 3, 5, 7 

## Source Code
program membuat tukar kolom jadi baris dan baris jadi kolom:
        
        #include <iostream>
        using namespace std;

        int main(){
          cout<<"Nama  : Herdin Kristianjani Zebua"<<endl;
          cout<<"NIM   : 1227050053"<<endl;
          cout<<"Kelas : IF-B"<<endl;
          cout<<endl;

          int i, j, m, n, matriks[10][10], transpose[10][10];

          cout << "Masukkan jumlah baris yang diinginkan: ";
          cin >> m;
          cout << "Masukkan jumlah kolom yang diinginkan: ";
          cin >> n;

          cout << "Masukkan nilai\n";
          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              cin  >> matriks[i][j];
            }
          }

          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              transpose[j][i] = matriks[i][j];
            }
          }

          cout << "Hasil pertukaran Matriks: \n";
          for (i = 0; i < n; i++){
            for (j = 0; j < m; j++){
              cout << transpose[i][j] << "\t";
            }
            cout << endl;
          }
        }
program menampilkan bilangan yang habis dibagi 3, 5, dan 7 pada data array dua dimensi:

        #include <iostream>
        using namespace std;

        const int MAX_ROWS = 100;
        const int MAX_COLS = 100;

        int main(){
          cout<<"Nama  : Herdin Kristianjani Zebua"<<endl;
          cout<<"NIM   : 1227050053"<<endl;
          cout<<"Kelas : IF-B"<<endl;

          int array[MAX_ROWS][MAX_COLS];
          int rows, cols;

          cout << "Masukkan jumlah baris array: ";
          cin >> rows;
          cout << "Masukkan jumlah kolom array: ";
          cin >> cols;

          cout << "Masukkan elemen-elemen array: " << endl;
          for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
              cin >> array[i][j];
            }
          }

          cout << "Bilangan yang habis dibagi 3, 5, dan 7: " << endl;
          for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
              if (array[i][j] % 3 == 0 && array[i][j] % 5 == 0 && array[i][j] % 7 == 0) {
                cout << array[i][j] << " ";
              }
            }
          }

          return 0;
        }
## Output
![Screenshot (50)](https://user-images.githubusercontent.com/115415378/208372360-5b7cc4f4-7118-4676-9f1f-448ce493f7d7.png)

![Screenshot (51)](https://user-images.githubusercontent.com/115415378/208372416-be0d51a3-beb0-46e8-93ad-2a35ca0a4859.png)


