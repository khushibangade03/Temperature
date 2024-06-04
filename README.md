import java.util.Scanner;
 
 public class Temperature{
	 
     public static void main(String[] args){
	   Scanner scanner =new Scanner(System.in)
;
	   System.out.println("please enter the temperature");
	    double  temp =scanner.nextDouble();
		
	   System.out.println("please enter the unit of temperature i.e. 'celsius' or 'kelvin' or 'fahrenheit' ");
	   String unit=scanner.next();
	   double kel=0;
	   double fah=0;
	   double cel=0;
	   
	   if(unit.equals("celsius")){
		   kel = (temp + 273.15);
		   System.out.println(kel + " °K");
		   fah = (temp * (9/5)) + 32.00;
		   System.out.println(fah + " °F");
		   }
		   
	   if(unit.equals("kelvin")){
		   cel = (temp - 273.15);
		   System.out.println(cel + " °C");
		   fah = (1.8*(temp-273.15))+32.00;
		   System.out.println(fah + " °F");
		   }  
		   
	   if(unit.equals("fahrenheit")){
		   cel = (temp -32.00 ) * 5/9;
		   System.out.println(cel + " °C");
		   kel = (temp + 459.67 ) * 5.00/9.00;
		   System.out.println(kel + " °K");
		   }   
		   

        }
 }
