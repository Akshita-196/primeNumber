# primeNumber
package primenumber;
import java.util.*;
public class PrimeNumber {

    public static void main(String[] args) {
        int flag=0;
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter a number:");
        int n=sc.nextInt();
        for(int i=2;i<=n/2;i++){
            if(n%i==0){
                flag=1;
                break;
            }
        }
        if(n==1){
            System.out.println("1 is neither prime nor composite number");
        }
        else{
            if(flag==0){
                System.out.println(n +" is prime number");
            }
            else{
                System.out.println(n +" is not prime number");
            }
        }
    }
    
}
