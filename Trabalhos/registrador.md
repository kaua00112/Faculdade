
import javax.swing.JOptionPane;
public class a222 {
	
	public static void main(String[]args) {
		
		double soma = 0;
		double soma1 = 0;
		int cont = 0;
		while(true) {
		Object[] possibilities = {"Receitas", "Despesas"};
		String mensagem = (String)JOptionPane.showInputDialog(null, "Escolha uma opусo:\n", "Registro", JOptionPane.PLAIN_MESSAGE, null, possibilities, "Receitas");
		String mensagem1 = (mensagem);


​		
​		
		if(mensagem1.equals("Receitas")) {
			String descrec = JOptionPane.showInputDialog(null, "informe a descriусo da receita:\n");
			String descrec1 = (descrec);
			System.out.println("Descriусo da receita:" + descrec1);


​			
			String receita = JOptionPane.showInputDialog("informe o valor da receita:\n");
			Double receita1 = Double.valueOf(receita);
			
			System.out.println("Valor da receita:" + receita1);
			
			if (receita1>=0) {
			soma = receita1 + soma;
			cont++;
			
			}


​			
​			
			String confirm = JOptionPane.showInputDialog("Deseja continuar adicionando informaушes?S/N");
			String confirm1 = (confirm);
			
			if(confirm1.equals("S"));
			if(confirm1.equals("N")) {
				System.out.println("Soma total das receitas:" + " " + soma);
				System.out.println("Descriусo da receita:" + descrec1);	
				System.out.println("Saldo atual:" + (soma - soma1));
				System.out.println("Soma total das despesas:" + " " + soma1);
				if(cont>1) 
					System.out.println("NЩmero de receitas e despesas registradas:" + " " + cont);
				break;
			}
		}


​	
			if (mensagem1.equals("Despesas")) {
			String descdes = JOptionPane.showInputDialog("informe a descriусo da despesa:\n");
			String descdes1 = (descdes);
			
			System.out.println("Descriусo da despesa:" + descdes1);


​			
		    String despesa = JOptionPane.showInputDialog("informe o valor da despesa:");
		    double despesa1 = Double.valueOf(despesa);
		    System.out.println("Valor da despesa:" + despesa1);
		    
		    if (despesa1>=0) {
			soma1 = despesa1 + soma1;
			cont++;
		    }


​			
​		    
		    String confirm2 = JOptionPane.showInputDialog("Deseja continuar adicionando informaушes? S/N");
			String confirm3 = (confirm2);
			
			if(confirm3.equals("S"));
			if(confirm3.equals("N")) {
				System.out.println("descriусo da despesa:" + descdes1);
				System.out.println("Soma total das despesas:" + " " + soma1);
				System.out.println("Soma total das receitas:" + " " + soma);
				System.out.println("Saldo atual:" + (soma - soma1));
				if(cont>1) 
					System.out.println("NЩmero de receitas e despesas registradas:" + " " + cont);
				break;
			}


​		   
			}


​    	      
​    	      
​	
​			
		}


​		  		  		    
​		
​		
		}
}
	


​		
​				
​			
​		
​		
​            
​		
​		
​		
​	
​		
​		
​	



