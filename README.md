# UAS-Dasprog_B

# Ujian Akhir Semester 1 
<br>Mata Kuliah 	:Dasar Pemrograman
<br> Nama		: Muhammad Miftahur Rizki A
<br>NIM		:	1227050090
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Pada UAS ini kami diminta untuk membuat 2 program, yang pertama program array dua dimensi dengan menukar(tranpose)baris menjadi kolom dan sebaliknya, dan program kedua yaitu program array dua dimensi dengan angka yang di inputnya habis di bagi 3,5,7.
## Source Code 1
    #include <iostream>
    using namespace std;

    void perkenalan();
    int main() {
      perkenalan();
     int arr[10][10], transpose[10][10], baris, kolom;

     cout << "Inputkan jumlah baris: ";
     cin >> baris;
     cout << "Inputkan jumlah kolom: "; 
     cin >> kolom;

     for(int i=0; i<baris; i++){
      for(int j=0; j<kolom; j++){
       cout << "baris "<<i+1<<" Kolom "<<j+1<<"="; cin >> arr[i][j];
      }
     }

     cout <<endl<<"Sebelum transpose"<< endl;

     for(int i=0; i<baris; i++){
      for(int j=0; j<kolom; j++){
       cout << arr[i][j] << " ";
      }
      cout << endl;
     }

     cout <<"Sesudah transpose"<< endl;

     for(int i=0; i<baris; i++){
      for(int j=0; j<kolom; j++){
       transpose[j][i] = arr[i][j];
      }
     }

     for(int i=0; i<kolom; i++){
      for(int j=0; j<baris; j++){
       cout << transpose[i][j] << " "; 
      }
      cout << endl;
     }
    }
    void perkenalan(){
      cout<<"--------------------------------------\n";
      cout<<"---------M Miftahur Rizki A-----------\n";
      cout<<"-------------1227050090---------------\n";
      cout<<"--------Informatika Kelas B-----------\n";
      cout<<"Program Matrix kolom menjadi baris  ><\n";
      cout<<"--------------------------------------\n";
    }
                                                                                                                                                                                           
## output 1
<img width="383" alt="image" src="https://user-images.githubusercontent.com/120999827/208482370-43c1bbd4-1859-4b95-a45e-8aa9e05dfbd5.png">


## Source Code 2 
    #include <iostream>
    using namespace std;
    void perkenalan();
    int main(){
        perkenalan();
      int arr[100][100], a, b, baris, kolom;

      cout<<" Input jumlah baris: "; 
    cin>>baris;
      cout<<" Input jumlah kolom: "; 
    cin>>kolom;
      cout << endl;

      for(a = 0; a < baris; a++){
          for(b = 0; b < kolom; b++){
              cout << " Baris " <<a+1<<", Kolom "<<b+1<< " = ";
              cin >> arr[a][b];
          }
          cout << endl;
      }

      cout << " Hasil input nilai : " << endl;

      for(a = 0; a < baris ; a++){
      for(b = 0; b < kolom; b++){
          cout << arr[a][b] << " ";
      }
      cout << endl;
      }

      cout << " Hasil bilangan yang habis dibagi 3,5,7 : " << endl;

      for(a = 0; a < baris ; a++){
      for(b = 0; b < kolom; b++){
          if(arr[a][b] % 3 == 0 || arr[a][b] % 5 == 0 || arr[a][b] % 7 == 0){
          cout << arr[a][b] << " ";
          }
          else{
            cout<<"-";
      }
      }
      cout << endl;
      }
      cout << endl;
    }
    void perkenalan(){
      cout<<"--------------------------------------\n";
      cout<<"---------M Miftahur Rizki A-----------\n";
      cout<<"-------------1227050090---------------\n";
      cout<<"--------Informatika Kelas B-----------\n";
      cout<<"--Program Matrix(habis dibagi 3,5,7)--\n";
      cout<<"--------------------------------------\n";
    }                                                                                                                                                                  
## Output 2
<img width="328" alt="image" src="https://user-images.githubusercontent.com/120999827/208481876-9cd27bd8-dc2e-471f-a5b4-1c9e5955237c.png">


