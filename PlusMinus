import java.io.*;
import java.math.*;
import java.security.*;
import java.text.*;
import java.util.*;
import java.util.concurrent.*;
import java.util.function.*;
import java.util.regex.*;
import java.util.stream.*;
import static java.util.stream.Collectors.joining;
import static java.util.stream.Collectors.toList;

class Result {

    /*
     * Complete the 'plusMinus' function below.
     *
     * The function accepts INTEGER_ARRAY arr as parameter.
     */

    public static void plusMinus(List<Integer> arr) {
    int pos = 0, neg = 0, zero = 0, n = arr.size();
    
    for(int i = 0; i< n;i++)
    {
        if(arr.get(i)<0)neg++;
        else if(arr.get(i)>0)pos++;
        else zero++;
        
    }
    double ratioPos=pos/(1.0*n), ratioNeg=neg/(1.0*n), ratioZero=zero/(1.0*n);
    
    System.out.println(String.format("%.6f",ratioPos));
    System.out.println(String.format("%.6f",ratioNeg));
    System.out.println(String.format("%.6f",ratioZero));

    }

}

public class Solution {
    public static void main(String[] args) throws IOException {
        BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(System.in));

        int n = Integer.parseInt(bufferedReader.readLine().trim());

        List<Integer> arr = Stream.of(bufferedReader.readLine().replaceAll("\\s+$", "").split(" "))
            .map(Integer::parseInt)
            .collect(toList());

        Result.plusMinus(arr);

        bufferedReader.close();
    }
}
