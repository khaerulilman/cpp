# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Mochammad khaerul ilman
<br>NIM		        :	1227050073
<br>Jurusan	    	:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
program dibawah ini adalah membuat matriks dengan menginputkan baris dan kolom ,kemudia akan dicari elemen elemen yang habis dibagi 3 ,5 ,7 dan yang tidak bisa dibagi dengan 3,5,7 akan menampilkan strip

## Source Code

```
#include <iostream>
#include <iomanip>
using namespace std;
int main()
{

    int jumlahBaris, jumlahKolom, i, j, baris, kolom;

    cout << "Input jumlah baris: ";
    cin >> jumlahBaris;
    cout << "Input jumlah kolom: ";
    cin >> jumlahKolom;
    cout << endl;

    int arr[jumlahBaris][jumlahKolom];

    for (i = 1; i <= jumlahBaris; i++)
    {
        for (j = 1; j <= jumlahKolom; j++)
        {
            cout << "Elemen matrik A baris ke-" << i << " kolom ke-" << j << ": ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

    cout << "Hasil input nilai : " << endl;

    for (i = 1; i <= jumlahBaris; i++)
    {
        for (j = 1; j <= jumlahKolom; j++)
        {
            cout << setw(3) << arr[i][j] << " ";
        }
        cout << endl;
    }

    cout << "Hasil bilangan yang habis dibagi 3,5,7 : " << endl;

    for (i = 1; i <= jumlahBaris; i++)
    {
        for (j = 1; j <= jumlahKolom; j++)
        {
            if (arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0)
            {
                cout << setw(3) << arr[i][j] << " ";
            }
            else
            {
                cout << " - ";
            }
        }
        cout << endl;
    }
    cout << endl;
}

```

## Output

//contoh output 
```
Input jumlah baris: 3
Input jumlah kolom: 4

Elemen matrik A baris ke-1 kolom ke-1: 3
Elemen matrik A baris ke-1 kolom ke-2: 5
Elemen matrik A baris ke-1 kolom ke-3: 2
Elemen matrik A baris ke-1 kolom ke-4: 4

Elemen matrik A baris ke-2 kolom ke-1: 2
Elemen matrik A baris ke-2 kolom ke-2: 5
Elemen matrik A baris ke-2 kolom ke-3: 2
Elemen matrik A baris ke-2 kolom ke-4: 5

Elemen matrik A baris ke-3 kolom ke-1: 2
Elemen matrik A baris ke-3 kolom ke-2: 5
Elemen matrik A baris ke-3 kolom ke-3: 2
Elemen matrik A baris ke-3 kolom ke-4: 5

Hasil input nilai : 
  3   5   2   4 
  2   5   2   5 
  2   5   2   5 
Hasil bilangan yang habis dibagi 3,5,7 : 
  3   5  -  - 
 -   5  -   5 
 -   5  -   5 
 
 ```
