# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Arief Rahman Mubarok
<br>NIM		:	1227050026
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

tema dari source code ini adalah array 2 dimensi menggunakan bahasa c++.
tujuan dari source code ini yaitu mencari nilai yang tidak habis dibagi 3, 5, dan 7 dari nilai yang diinputkan pada baris dan kolom.
<br> Algoritma dari source code ini yaitu : 
<br> 1. input jumlah baris yang diinginkan
<br> 2. input jumlah kolom yang diinginkan
<br> 3. input satu persatu nilai pada baris dan kolom
<br> 4. akan ditampilan angka yang sudah diinput sesuai dengan tampilan matriks dan angka yang tidak habis dibagi 3, 5, dan 7.

## Source Code
      #include <iostream>
      using namespace std;
      int main (){
      int array [20][20];
      int b, k, i, j;
      cout << "Masukkan jumlah baris : ";
      cin >> b;
      cout << "Masukkan jumlah kolom : ";
      cin >> k;

      for (i=0;i<=b-1;i++) {
        for(j=0;j<=k-1;j++) {
          cout << "baris ke "<<i+1<<" kolom ke "<<j+1<<" : " ;
          cin >>array[i][j];
        }
      }
      cout << "Nilai yang diinputkan : \n";
      for(int i = 0; i < b; i++){
        for(int j = 0; j < k; j++){
          cout<< array[i][j]<<"\t";
        }
        cout<<endl;
      }
      int angka[20];
      int index = 0;
      for(i=0;i<b;i++){
        for(j=0;j<k;j++) {
          if (array [i][j]%3 != 0 && array[i][j]%5 != 0 && array[i][j]%7 != 0){
            angka[index] = array[i][j];
            index++;
          }
        }
      }
      cout<<"Angka yang tidak bisa dibagi 3, 5, 7 adalah ";
      for(int i = 0; i < index; i++){
        cout<<angka[i]<<", ";

      }
    }

## Output

<img width="673" alt="buat uas" src="https://user-images.githubusercontent.com/118902896/209269714-d02b52ff-2ed5-4448-86e6-3129475fe61e.png">
