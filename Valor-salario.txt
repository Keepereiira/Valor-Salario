package valorsalario;
import java.util.Scanner;

public class Valorsalario {

    public static void main(String[] args) {
        Scanner dados = new Scanner(System.in);
        int salario1,salario2,salario3,salario4, media;
        
        String funcionario, funcionario1, funcionario2, funcionario3;
        
        System.out.println("Digite o nome do seu primeiro funcionario");
        funcionario1 = dados.next();
        System.out.println("Digite o nome do seu segundo funcionario");
        funcionario2 = dados.next();
        System.out.println("Digite o nome do seu terceiro funcionario");
        funcionario3 = dados.next();
        System.out.println("Digite o nome do seu quarto funcionario");
        funcionario4 = dados.next();
        System.out.println("Digite o salario do primeiro funcionario");
        salario1 = dados.nextInt();
        System.out.println("Digite o salario do segundo funcionario");
        salario2 = dados.nextInt();
        System.out.println("Digite o salario do terceiro funcionario");
        salario3 = dados.nextInt();
        System.out.println("Digite o salario do quarto funcionario");
        salario4 = dados.nextInt();
        media = (salario1 + salario2 + salario3 + salario4)  / 4;
        System.out.println("A media dos salarios é " + media);
    }
}

Segundo app:
package segundoapp;

import java.util.Scanner;

public class segundoapp {

   
    public static void main(String[] args) {
        Scanner dados = new Scanner(System.in);
        float salario, media;

        System.out.println("Digite seu salario");
        salario = dados.nextFloat();

        if (salario <= 1693.72) {
            media = salario * 0.08f;

        } else if (salario >= 1693.73 && salario < 2822.90) {
            media = salario * 0.09f;

        } else if (salario >= 2822.91 && salario < 5646.80) {
            media = salario * 0.11f;
        } else {
            media = 621.04f;
        }
        System.out.println("O seu salario é " + (salario - media));
    }
}
