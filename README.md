# jurnnal-no-2
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

package jurnal.pkg2;

import java.util.Scanner;


public class Jurnal2 {


    public static void main(String[] args) {
        int awal,akhir;
        boolean bujur;
        Scanner in = new Scanner (System.in);
        System.out.print ("masukkan angka awal : ");
        awal = in.nextInt();
        System.out.print ("masukkan angka akhir : ");
        akhir =in.nextInt ();
        System.out.print ("Angka prima antara " + awal + " sampai " +akhir+ " adalah : ");
        for (int a = awal; a <=akhir; a++){
            bujur = false ;
            if(a == 2){
                bujur = true ;
            }
            else{
                for (int b = 2 ; b < a; b++){
                    if (a % b == 0){
                        bujur = false;
                        break;
                    }else{
                        bujur= true;
                    }
                }
            }
            if(bujur){
                System.out.printf(a + " ");
            }
        }
    }
    
}
