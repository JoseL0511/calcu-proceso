# calcu-proceso
package calc;

import java.util.Scanner;

		public class calc {

			public static void main(String[] args) {
				// TODO Auto-generated method stub
			   int c=0, e=0, res=0;
			   char sign=' ';
			   String oper=" ";
			   String sel=null;
			   Scanner scan=new Scanner(System.in);	
		       System.out.println("seleccione la opcion\n");
		       System.out.println("1: suma"
		    		   + "\n2: resta"
		    		   + "\n3: multiplicacion"
		    		   + "\n4: division");
		       sel=scan.next();
		       
		       switch(sel){
		       case "1":
		    	   System.out.println("ha seleccionado suma");
		    	   System.out.println("ingrese el primer numero");
		    	   c=scan.nextInt();
		    	   System.out.println("ingrese el segundo numero");
		    	   e=scan.nextInt();
		    	   
		    	   suma s = new suma(c, e);
					res = s.getRes();
					sign = s.getSign();
					oper = s.getOperation();
		    	   System.out.println("el resultado de la "+oper+" "+c+" "+sign+" "+e+" es igual a: "+res);
		    	   break;
		       case "2":
		    	   System.out.println("ha seleccionado resta");
		    	   System.out.println("ingrese el primer numero");
		    	   c=scan.nextInt();
		    	   System.out.println("ingrese el eegundo numero");
		    	   e=scan.nextInt();
		    	   
		    	   resta r = new resta(c, e);
					res = r.getRes();
					sign = r.getSign();
					oper = r.getOperation();
		    	   System.out.println("el resultado de la "+oper+" "+c+" "+sign+" "+e+" es igual a: "+res);
		    	   break;
		       case "3":
		    	   System.out.println("ha seleccionado multiplicacion");
		    	   System.out.println("ingrese el primer numero");
		    	   c=scan.nextInt();
		    	   System.out.println("ingrese Eel segundo nmero");
		    	   e=scan.nextInt();
		    	   
		    	   multiplicacion m = new multiplicacion(c, e);
					res = m.getRes();
					sign = m.getSign();
					oper = m.getOperation();
		    	   System.out.println("el resultado de la "+oper+" "+c+" "+sign+" "+e+" es igual a: "+res);
		    	   break;
		       case "4":
		    	   System.out.println("ha deleccionado division");
		    	   System.out.println("ingrese el primer numero");
		    	   c=scan.nextInt();
		    	   System.out.println("ingrese el segundo numero");
		    	   e=scan.nextInt();
		    	   
		    	   division d = new division(c, e);
					res = d.getRes();
					sign = d.getSign();
					oper = d.getOperation();
		    	   System.out.println("el resultado de la "+oper+" "+c+" "+sign+" "+e+" es igual a: "+res);
		    	   break;
		       default:
		    	   System.out.println("no existe");
		       scan.close();
		       }   	   
			}
		}
