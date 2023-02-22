import java.util.Scanner;

public class HavaDurumu {
	
public static void main(String[] args) {

double havaSicakligi;


    Scanner scanner = new Scanner(System.in);
    System.out.print("Hava Sıcaklığını Giriniz : ");
    havaSicakligi = scanner.nextDouble();

    if(havaSicakligi>=0 && havaSicakligi<=35) {
        if (havaSicakligi < 5) {
            System.out.println("Kayak yapabilirsiniz");
        } else {
            if (havaSicakligi <= 15) {
                System.out.println("Sinemaya gidebilirsiniz");
            } else {
                if (havaSicakligi <= 25) {
                    System.out.println("Piknik yapabilirsiniz");
                } else {
                    System.out.println("Yüzebilirsiniz");
                }
            }
        }
    }
    else{
        System.out.println("Dışarı çıkmamanızı öneririz");
    }
}
}
