# chef-and-string
getting error
Exception in thread “main” java.util.NoSuchElementException
at java.util.Scanner.throwFor(Scanner.java:862)
at java.util.Scanner.next(Scanner.java:1485)
at java.util.Scanner.nextInt(Scanner.java:2117)
at java.util.Scanner.nextInt(Scanner.java:2076)
at Codechef.main(Main.java:15)

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be “Main” only if the class is public. */
class Codechef
{
public static void main (String[] args) throws java.lang.Exception
{

Scanner sc = new Scanner(System.in);

int N = sc.nextInt();

int s[] = new int[N];
for(int j=0; j<N; j++){
  s[j] = sc.nextInt();
}
sc.close();

int temp = 0;
for(int i=0; i<s.length-1; i++){
  if(s[i]<s[i+1]){
    temp = temp+((s[i+1]-s[i])-1);
  }else{
    temp = temp+((s[i]-s[i+1])-1);
  }
}System.out.println(temp);

}
}
