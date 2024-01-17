# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Mochammad khaerul ilman
<br>NIM		        :	1227050073
<br>Jurusan	    	:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
program dibawah ini adalah program membuat suatu matriks dengan menginputkan kolom dan baris , lalu matriks tersebut akan ditampilkan kemudian matriks tersebut akan di transpose kan


## Source Code

```
#include <iostream>
  
using namespace std;
  
int main()
{
    cout << "BIODATA : " << endl;
    cout << "Nama : Mochammad khaerul ilman" << endl;
    cout << "Nim  : 1227050073" << endl;
    cout << "Kelas: IF-B" << endl
         << endl;
    cout << "===Program Transpose Matrix===" << endl;
    cout << endl;

    int i, j, k, baris, colom;

    cout << "masukan baris = ";
    cin >> baris;
    cout << "masukan colom = ";
    cin >> colom;
    cout << endl;
    double a[baris][colom];

    cout << endl
         << "Elemen matriks A : " << endl;
    for (i = 1; i <= baris; i++)
    {
        for (j = 1; j <= colom; j++)
        {
            cout << "Elemen matrik A baris ke-" << i << " kolom ke-" << j << ": ";
            cin >> a[i][j];
        }
        cout << endl;
    }

    cout << endl;

    cout << "Element matriks A adalah : " << endl<< endl;
    for (i = 1; i <= baris; i++)
    {
        for (j = 1; j <= colom; j++)
        {
            cout << "    " << a[i][j];
        }
        cout << endl;
    }
    cout << endl;
    cout << endl;
    cout << "Matriks A di Transpose :" << endl;
    for (i = 1; i <= colom; i++)
    {
        // if ()
        for (j = 1; j <= baris; j++)
        {
            cout << "    " << a[j][i];
        }
        cout << endl;
    }
    return 0;
}
```

## Output
```
//contoh output

BIODATA : 
Nama : Mochammad khaerul ilman
Nim  : 1227050073
Kelas: IF-B

===Program Transpose Matrix===

masukan baris = 4
masukan colom = 2


Elemen matriks A : 
Elemen matrik A baris ke-1 kolom ke-1: 3
Elemen matrik A baris ke-1 kolom ke-2: 2

Elemen matrik A baris ke-2 kolom ke-1: 4
Elemen matrik A baris ke-2 kolom ke-2: 2

Elemen matrik A baris ke-3 kolom ke-1: 4
Elemen matrik A baris ke-3 kolom ke-2: 1

Elemen matrik A baris ke-4 kolom ke-1: 3
Elemen matrik A baris ke-4 kolom ke-2: 5


Element matriks A adalah : 

    3    2
    4    2
    4    1
    3    5


Matriks A di Transpose :
    3    4    4    3
    2    2    1    5

```




