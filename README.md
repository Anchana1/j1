# j1import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Input the total number of factories and their values
        int n = scanner.nextInt();
        int[] values = new int[n];

        for (int i = 0; i < n; i++) {
            values[i] = scanner.nextInt();
        }

        // Calculate the net worth
        int netWorth = 0;
        for (int value : values) {
            netWorth += value;
        }

        // Output the net worth
        System.out.println(netWorth);

        scanner.close();
    }
}
