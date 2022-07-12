# java-program
import java.util.Scanner;

public class bill 
{
    public static void main(String args[])
    {
        Scanner s=new Scanner(System.in);
        
        String name,date,blno;
        int slno;
        double qty,pr,amt,taxp,tamt,tot,dis,net;
        
        System.out.print("Enter The Bill No");
        blno=s.nextLine();
        System.out.print("Enter The Date");
        date=s.nextLine();
        System.out.print("Enter The Date Item Name");
        name=s.nextLine();
        
        System.out.print("Enter The Serial No");
        slno=s.nextInt();
        
        System.out.print("Enter The Quantity");
        qty=s.nextDouble();
        System.out.print("Enter The Price");
        pr=s.nextDouble();
        
        System.out.print("Enter The Tax Percentage");
        taxp=s.nextDouble();
        tamt=qty*pr*taxp/100;
        tot=qty*pr+tamt;
        System.out.print("Enter The Discount");
        dis=s.nextDouble();
        net=tot-dis;
        System.out.println("\t\t\tMargin Free Market");
        System.out.println("\t\t\t      Kottayi");
        System.out.println("\t\t\t     Palakkad");
        System.out.println("\t\t\t      Kerala");
        System.out.println("\t\t\t   Pin - 678572");
        System.out.println("\t\t\t*******************");
        System.out.println("\tBill No :"+blno+"  \t\t\t\t Date :"+date);
        System.out.println("\t-------------------------------------------------------------");
        System.out.println("\tSl No \t Name \t Qty \t Price \t Tax% \t Tamt \t Amount");
        System.out.println("\t-------------------------------------------------------------");
        System.out.println("\t"+slno+" \t "+name+" \t "+qty+" \t "+pr+" \t "+taxp+" \t "+tamt+" \t "+tot+"");
        System.out.println("\n\n\t=============================================================");
        System.out.println("\t\t\t\t\t\tAmount     "+tot);
        System.out.println("\t\t\t\t\t\tDiscount   "+dis);
        System.out.println("\t\t\t\t\t\tNet Total  "+net);
        System.out.println("\t=============================================================");
        System.out.println("\t=================Thank You Visit Again=======================");
        
    }
}
