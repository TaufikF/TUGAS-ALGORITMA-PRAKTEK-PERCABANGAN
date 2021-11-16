# TUGAS-ALGORITMA-PRAKTEK-PERCABANGAN

// TUGAS KULIAH


#include <iostream>
	
// itu abis include diatas dikasih iostream ya, sebenernya udh ditulis tapi gak tampil, gak tau lh tulis aja :) #SALAMDARIYGBUAT

using namespace std;
  
int main() {

  
	/*	1 Membaca sebuah bilangan bulat antara 1 sampai 4, lalu mencetak tulisan dari angka tersebut.
		Contoh: Jika diinput angka 1 maka output akan tercetak tulisan SATU
		jika di input selain dari 1 sampai 4 maka munculkan pesan "Anda Salah memasukan Input
		Kode"	
		
	*/
	
  	// DEKLARASI VARIABEL
  
	int angka;
	cout << "Masukan angka 1 - 4 = "; cin >> angka;
  
  
  	// ALGORITMANYA 
	
	if ( angka == 1 ) {
		cout << "SATU";
	} else if ( angka == 2 ) {
		cout << "DUA";
	} else if ( angka == 3 ) {
		cout << "TIGA";
	} else if ( angka == 4 ) {
		cout << "EMPAT";
	} else {
		cout << "Anda salah memasukan input kode";
	}
	
	
	
	/*	2 Buatlah program untuk menentukan jumlah hari dalam bulan
	*/
	
	
	// DEKLARASI VARIABEL
	
	int bulan, tahun, j_hari;
	
	cout << "Masukan bulan 1 - 12  = "; cin >> bulan;
	cout << "Masukan tahun         = "; cin >> tahun;
	
	cout << "~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n";
	
	
	// MENENTUKAN JUMLAH HARI JIKA ADA TAHUN KABISAT
	
	if ( bulan == 2 ) {
		
		if ( tahun % 4 == 0 ) {
			j_hari = 29;
			cout << "29 hari / tahun kabisat\n" << endl;
			cout << "Bulan " << bulan; cout << " Tahun " << tahun << "\n";
			cout << "Jumlah hari = " << j_hari << " hari";
		} else {
			j_hari = 28;
			cout << "28 hari / tahun biasa\n" << endl;
			cout << "Bulan " << bulan; cout << " Tahun " << tahun << "\n";
			cout << "Jumlah hari = " << j_hari << " hari";
		}
				
	
	// MENENTUKAN JUMLAH HARI DALAM SETIAP BULAN KECUALI FEBRUARI 	
	
	} else if ( bulan == 1 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
		
	} else if ( bulan == 3 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 4 ) {
		j_hari = 30;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 5 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 6 ) {
		j_hari = 30;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 7 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 8 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 9 ) {
		j_hari = 30;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 10 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 11 ) {
		j_hari = 30;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else if ( bulan == 12 ) {
		j_hari = 31;
		cout << "Bulan ke " << bulan; cout << " Tahun ke " << tahun << "\n";
		cout << "Jumlah hari = " << j_hari << " hari";
	
	} else {
		cout << "Bulan tidak tersedia";
	}

	
	
	/*	3. Mencari hari kelahiran seseorang . Hari lahir kelahiran, sebagian orang pasti banyak yang
		tahu hari apa dia dilahirkan. Buat program untuk mencari hari kelahiran
	*/



	/* PROGRAM MENCARI HARI LAHIR */
	
	cout << "--- ******************************** ---\n";
	cout << "---    PROGRAM MENCARI HARI LAHIR    ---\n";
	cout << "--- ******************************** ---\n";
	cout << "****************************************\n";

	// DEKLARASI VARIABEL
	
	int tgl_lahir, bln_lahir, thn_lahir, x, y, z, sisa;

	// MENGINPUTKAN TGL_LAHIR, BLN_LAHIR DAN THN_LAHIR
	
	cout << "Masukan Tanggal Lahir 	= "; cin >> tgl_lahir;
	cout << "Masukan Bulan Lahir 	= "; cin >> bln_lahir;
	cout << "Masukan Tahun Lahir 	= "; cin >> thn_lahir;
	
	
	// MENENTUKAN TAHUN KABISAT
	
	if ( thn_lahir % 4 != 0 )  {
		x = 28;
		if ( (thn_lahir % 100 == 0) && (thn_lahir % 400 != 0) ) {
			x = 28;	
		}	
	} else {
		x = 29;	
	}
	
	// MENCARI JUMLAH HARI DARI 1 JANUARI SAMPAI BULAN DAN TANGGAL LAHIR ANDA
	
	if ( bln_lahir == 1 ) {
		cout << tgl_lahir << " Januari adalah hari ke  -> " << tgl_lahir;
	} else if ( bln_lahir == 2 ) {
		y = 31 + tgl_lahir;
		cout << tgl_lahir << " Februari adalah hari ke -> " << y;
	} else if ( bln_lahir == 3 ) {
		y = 31 + x + tgl_lahir;
		cout << tgl_lahir << " Maret adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 4 ) {
		y = 31 + x + 31 + tgl_lahir;
		cout << tgl_lahir << " April adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 5 ) {
		y = 31 + x + 31 + 30 + tgl_lahir;
		cout << tgl_lahir << " Mei adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 6 ) {
		y = 31 + x + 31 + 30 + 31 + tgl_lahir;
		cout << tgl_lahir << " Juni adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 7 ) {
		y = 31 + x + 31 + 30 + 31 + 30 + tgl_lahir;
		cout << tgl_lahir << " Juli adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 8 ) {
		y = 31 + x + 31 + 30 + 31 + 30 + 31 + tgl_lahir;
		cout << tgl_lahir << " Agustus adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 9 ) {
		y = 31 + x + 31 + 30 + 31 + 30 + 31 + 30 + tgl_lahir;
		cout << tgl_lahir << " September adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 10 ) {
		y = 31 + x + 31 + 30 + 31 + 30 + 31 + 30 + 31 + tgl_lahir;
		cout << tgl_lahir << " Oktober adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 11 ) {
		y = 31 + x + 31 + 30 + 31 + 30 + 31 + 30 + 31 + 30 + tgl_lahir;
		cout << tgl_lahir << " November adalah hari ke - > " << y << "\n";
	} else if ( bln_lahir == 12 ) {
		y = 31 + x + 31 + 30 + 31 + 30 + 31 + 30 + 31 + 30 + 31 + tgl_lahir;
		cout << tgl_lahir << " Desember adalah hari ke - > " << y << "\n";
	} else {
		cout << "Bulan anda tidak ditemukan" << "\n";
	}
	
	
	cout << "**--------------------------------**\n";
	cout << "**--------------------------------**\n";
	
	
	// MENCARI SISA HARI 
	
	z 	 = (thn_lahir - 1) / 4;
	sisa = (thn_lahir + y + z) % 7;
	
	
	// MENENTUKAN HARI LAHIR DARI PERHITUNGAN SISA HARI
	
	if ( sisa == 0 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah Hari -> Jum'at";
	} else if ( sisa == 1 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah hari -> Sabtu";
	} else if ( sisa == 2 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah hari -> Minggu";
	} else if ( sisa == 3 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah hari -> Senin";
	} else if ( sisa == 4 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah hari -> Selasa";
	} else if ( sisa == 5 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah hari -> Rabu";
	} else if ( sisa == 6 ) {
		cout << tgl_lahir << " - " << bln_lahir << " - " << thn_lahir << ", Hari Lahir Anda Adalah hari -> Kamis";
	} else {
		cout << "Belajar lagi deq";
	}
  
  
}
