# my-first-java-code
import java.util.Scanner;

public class FruitPriceAlt {

	public static void main(String[] args) { 
		
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter the Fruit");
		String fn = sc.nextLine();
		System.out.println("Enter the quantity");
		int qty = sc.nextInt();
		int cost = 0;
		
		if(fn.equals("apple")) {
			
			if(qty<=20) {
				cost = qty*5;
				System.out.println(cost);
			}
			else {
				cost = qty*7;
				System.out.println(cost);
			}
		}
		else if(fn.equals("kiwi")) {
			
			if(qty<=10) {
				cost = qty*2;
				System.out.println(cost);
			}
			else {
				if((qty>10)&&(qty<=25)){
					cost = qty*4;
					System.out.println(cost);
				}
				else {
					cost = qty*6;
					System.out.println(cost);
				}
			}
		}
		
		else if(fn.equals("banana")) {
			
			if(qty<=100) {
				cost = qty*3;
				System.out.println(cost);
			}
			else {
				cost = qty*4;
				System.out.println(cost);
			}
		}
		
	}

}
