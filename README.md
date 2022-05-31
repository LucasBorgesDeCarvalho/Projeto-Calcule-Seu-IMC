# Projeto-Calcule-Seu-IMC
Descubra qual o valor do seu IMC e um pouco mais sobre sua Saúde!
import java.util.Scanner;

class Main {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("===========================================================");

        System.out.print("Digite seu Nome: ");
        String nome = sc.nextLine();

        System.out.println("\nOla " + nome + " a seguir calcule seu IMC");

        double peso, altura, imc;

        System.out.print("\nDigite o seu peso: ");
        peso = sc.nextDouble();

        System.out.print("\nDigite a sua altura: ");
        altura = sc.nextDouble();
        System.out.print("-----------------------------------------------------------");

        imc = peso/(altura*altura);

        System.out.println("\nOla " + nome + " :");
        System.out.printf("Seu IMC eh: %.2f\n", imc);


        if (imc <= 19) {
            System.out.println("Voce esta muito magro");
        }else
        if (imc >= 18.5 && imc <= 24.9) {
            System.out.println("Voce esta com o peso ideal");
        }else
        if (imc >= 25.0 && imc <= 29.9) {
            System.out.println("Voce esta com sobrepeso, consulte-se com um nutricionista");
        }else
        if (imc >= 30.0 && imc <= 39.9) {
            System.out.println("Voce esta com obeso, va ao medico para tratamento");
        }else
            System.out.println("Voce esta com obesidade, corra para o medico");

        System.out.println("===========================================================");
    }
}
