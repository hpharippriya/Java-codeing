# Java-codeing
import java.util.Scanner;

public class WordCount {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter the text:");
		String text = sc.nextLine();
		text = text.trim();
		int count;
		if (text.isEmpty()) {
			count = 0;
		} else {
			String[] words = text.split("\\s+");
			count = words.length;
		}
		System.out.println("Number of words in the text:" + count);
		sc.close();
	}
}
