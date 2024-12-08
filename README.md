# Power-function-02
Power function 02
import java.util.Scanner;

public class Power02 {
    public Power02() {
    }

    static int func(int base, int x) {
        return x == 0 ? 1 : base * func(base, x - 1);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int base = sc.nextInt();
        int x = sc.nextInt();
        int ans = func(base, x);
        System.out.println(ans);
    }
}
