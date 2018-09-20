# SalesWithDiscounts
SalesWithDiscounts
package Assignments;

	import java.util.Scanner;

	public class SaleWithDiscount {
	      public static void main(String[] args) {
			
	    	  Scanner scan = new Scanner(System.in);
	    	  System.out.println("Enter unit price for purchase");
	    	  
	    	  double unitPrice = scan.nextDouble();
	    	  System.out.println("Enter quantity of units");
	    	  double quantity = scan.nextDouble();
	    	  
	    	  double grandTotal;
	    	  double discount=0;
	    	  grandTotal = unitPrice*quantity;
	    	 
	      	  if (quantity>=100 && quantity <=120) {
	       		  discount = 10;
	       		System.out.println("Grand Total: "+"$"+grandTotal); 
	       		System.out.println("Discount : "+discount+" %");
	       		System.out.println("Discount applied "+ (grandTotal*discount)/100);
	       		System.out.println("Total : "+ (grandTotal - (grandTotal*discount)/100));
	        } else if (quantity > 120) {
	    		  discount = 15;
	    		  System.out.println("Grand Total: "+"$"+grandTotal); 
	         	  System.out.println("Discount : "+discount+" %");
	         	  System.out.println("Discount applied "+ (grandTotal*discount)/100);
	         	  System.out.println("Total : "+"$"+ (grandTotal - (grandTotal*discount)/100));
	      	  } else if(quantity<100) {
	    		  System.out.println("Discount rate is 0% "+"Grand Total: " +grandTotal);
	    	  }
		    	  scan.close();
		}
	}


