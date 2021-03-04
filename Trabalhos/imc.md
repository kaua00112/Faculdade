package condicional;

import javax.swing.JOptionPane;

public class imc {

	  public static void main (String[] args) {
		  String pesoComoTexto = JOptionPane.showInputDialog("informe seu peso");
		  double pesoComoDouble = Double.valueOf(pesoComoTexto);
		  
		  String alturaComoTexto = JOptionPane.showInputDialog("informe sua altura");
		  Double alturaComoDouble = Double.valueOf(alturaComoTexto);
		  
		  double imc = pesoComoDouble / (alturaComoDouble * alturaComoDouble);
		  
		  System.out.println("IMC"+String.format("%.2f",imc));
		  
		  /*Menos do que 18,5 Abaixo do peso
		  Entre 18,5 e 24,9 Peso normal
		  Entre 25 e 29,9 Sobrepeso
		  Entre 30 e 34,9 Obesidade grau 1
		  Entre 35 e 39,9 Obesidade grau 2
		  Mais do que 40 Obesidade grau 3*/
		  
		  if (imc <18.5) {
			  System.out.println("abaixo do peso");
			  
		  }else if (imc >=18.5 && imc <=24.9) {
			  System.out.println("Peso normal");
		  }else if (imc >= 25 && imc <= 29.9) {
			  System.out.println("Sobrepeso");
		  }else if (imc >= 30 && imc <= 34.9) {
			  System.out.println("Obesidade grau 1");
		  }else if (imc >= 35 && imc <= 39.9) {
			  System.out.println("Obesidade grau 2");			 
		  }else {
			  System.out.println("Obesidade grau 3");
		  }
			  
		 
		  

		  
		  
	  }
}
