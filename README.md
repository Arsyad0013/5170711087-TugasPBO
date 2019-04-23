# 5170711087_TugasPBO
Muhamad Arsyad
5170711087
TEKNIK ELEKTRO


A.	SOAL:
Membuat program dengan menerapkan teori pewarisan, metode overiding dan acces protected dengan kasus class pewaris adalah class manusia.

B.	KODING dan PENJELASAN:
1.	Class karakteristik

package pewarisan;


public class karakteristik {
    
    void tandamanusia (){
        System.out.println("Bisa Tertawa");
        System.out.println("Bisa Berpikir");
        System.out.println("Bisa Berjalan");
    }
    
}
 

•	Class Karakteristik adalah class induk.
•	Diatas ada method void tandamanusia.


2.	Class manusia

package pewarisan;


class manusia extends karakteristik  {
     void identitas (){
        System.out.println("Muhamad Arsyad");
        System.out.println("20 Tahun");
        System.out.println("Mahasiswa");
        System.out.println("Asal Banjarmasin");
    }
    @Override
    void tandamanusia (){
        System.out.println("Bisa Berenang");
        System.out.println("Bisa Berslancar"); 
    }
   
    protected manusia (){
        System.out.println("Pemalas");
        System.out.println("Pemarah");
        System.out.println("Mager");
        System.out.println("Males PENGEN BELI TRUK!");
        
    }

}
 

•	Class manusia adalah class pewaris dari class karakteristik.
•	Bisa dilihat pada koding (class manusia extends karakteristik).
•	Void tanda manusia memakai metode overriding karena methodnya sama dengan class induk (class karakteristik).
•	Pada method protected manusia kita menggunakan modifier protected yang artinya hanya bisa di akses oleh class, package, subclass. Tidak untuk world.

3.	Main Class

package pewarisan;


public class Pewarisan {

   
    public static void main(String[] args) {
        karakteristik x = new karakteristik ();
        manusia y = new manusia ();
        y.identitas();
        y.tandamanusia();
        x.tandamanusia();
       
       
        
    }
    
}

 

•	Jika ingin menjalankan program di atas maka kita harus mengkompile terlebih dahulu




 
