Penjelasan Tiap Baris Pemrograman

a.   import java.util.Scanner; 
   penjelasan : Mengimpor kelas Scanner dari library java.util yang digunakan untuk membaca input dari user (keyboard).
   
b.   Scanner scanner = new Scanner(System.in); 
   penjelasan : Objek Scanner tersebut dibuat untuk membaca input dari System.in (keyboard).
   
c.   String[] cabangOlahraga = {"Badminton", "Basket", "Bola Voli"}; :
   penjelasan : Program tersebut mendeklarasikan array string yang berisi nama-nama cabang olahraga.
   
d.   String[] atlet = new String[18]; 
   penjelasan : Mendeklarasikan array string bernama atlet dengan bernilai 18 untuk menyimpan 18 nama atlet.
   Keterangannya, Karena ada 3 cabang olahraga, setiap cabang diikuti oleh 2 Politeknik, dan setiap politeknik harus 
   menyertakan 3 atlet jadi kebutuhan yang dibutuhkan untuk penyimpanan ialah 18.
   
e.   Menginputkan nama menggunakan perulangan bersarang, pada baris :
  1. for (int i = 0; i < cabangOlahraga.length; i++) {
            System.out.println("Masukkan nama atlet untuk cabang " + cabangOlahraga[i] + ":");
   - Penjelasan Loop i : Iterasi melalui cabang olahraga. Iterasi pertama ini mengakses setiap cabang olahraga dalam array 
     cabang 
     olahraga, dan program nantinya akan meminta input untuk nama-nama atlet sesuai cabang olahraga.
  2. for (int j = 0; j < 2; j++) { 
                System.out.println("Politeknik " + (j + 1) + ":");
   - Penjelasan Loop j : Iterasi melalui dua politeknik untuk setiap cabang olahraga. Iterasi kedua memisahkan data 
     berdasarkan Politeknik (karena ada politeknik 1 dan politeknik 2 untuk setiap cabang olahraga).
  3. for (int k = 0; k < 3; k++) {  
                    String namaAtlet;
   - Penjelasan Loop k : Iterasi untuk memasukkan tiga nama atlet untuk setiap politeknik. Jika user memasukkan nama kosong 
     (tekan enter tanpa mengetik) maka program akan meminta user untuk menginput ulang nama atlet yang kosong sampai nama 
     yang valid di masukkan.
     
  f.   Menampilkan Data dari Array Atlet Menggunakan perulangan bersarang dimana, setelah semua nama atlet di inputkan,
     program akan menampilkan data yang telah di simpan.
     Baris Kode program :
     1. System.out.println("\nInformasi Nama Atlet:");
         for (int i = 0; i < cabangOlahraga.length; i++) {
             System.out.println("Cabang " + cabangOlahraga[i] + ":");
   - Penjelasan Iterasi Pertama : Untuk menampilkan nama cabang olahraga
     2. for (int j = 0; j < 2; j++) {
                System.out.println("Politeknik " + (j + 1) + ":");
   - Penjelasan Iterasi kedua : Menampilkan Politeknik 1 dan di lanjut politeknik 2
     3. for (int k = 0; k < 3; k++) {
                    System.out.println("Atlet " + (k + 1) + ": " + atlet[k]);
                }
            }
        }

    - Penjelasan Iterasi ketiga : Menampilkan nama-nama atlet dari politeknik yang suda di
    inputkan oleh user.
    
  g.  scanner.close();
        }
    }
    - penambahan scanner.close(); diakhir tersebut digunakan saat semua operasi input selesai agar tidak ada kebocoran 
      sumber data. 
     
