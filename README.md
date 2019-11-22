# program1
#difference of sum of odd place with sum of even place or vice versa
import java.util.Scanner;
public class oddeven
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int a[]=new int[100];
        int n,i,sum1=0,sum=0,result;
        System.out.println("enter the size of the array");
        n=sc.nextInt();
        System.out.println("enter the number");
        for(i=1;i<=n;i++)
        {
            a[i]=sc.nextInt();
        }
        for(i=1;i<=n;i=i+2)
        {
            sum+=a[i];
        }
        for(i=2;i<=n;i+=2)
        {
            sum1+=a[i];
        }
        if(sum>sum1)
        result=sum-sum1;
        else
        result=sum1-sum;
        System.out.println("the answer"+result);
    }
}
            
      

