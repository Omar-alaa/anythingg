import java.util.Scanner;
public class EuclidSGameJava {

   public static int GCD(int  n1,int n2){
       if(n2==0)
           return n1;
       else
           return GCD(n2, n1 % n2);
   
   }
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
         System.out.println(" please enter your first number ");
        int n1=scan.nextInt();
        System.out.println("  please enter your secound number  ");
        int n2=scan.nextInt();
       if(n1/GCD(n1, n2)%2!=0){
            System.out.println(" the first player win : ");
        }
        else
        System.out.println(" the secound player win  ");
    }
    
}
