# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Herdin Kristianjani Zebua
<br>NIM		        :	1227050053
<br>Jurusan	    	:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

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


