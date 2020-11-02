# java
import javax.swing.JOptionPane;

/**
 *
 * @author Fawad Sarim
 */
public class Resistance {
    String digit_band1_color;
    String digit_band2_color;
    String multiplier_band3_color;
    String tolerance_band4_color;
    int temp1,temp2,temp3;
    double temp4;
    double result;
    public Resistance(String a,String b,String c,String d){
        digit_band1_color=a;
        digit_band2_color=b;
        multiplier_band3_color=c;
        tolerance_band4_color=d;
        switch (digit_band1_color){
            case "Black":
                temp1=0;
                break;
            case "Brown":
                temp1=1;
                break;
            case "Red":
                temp1=2;
                break;
            case "Orange":
                temp1=3;
                break; 
            case "Yellow":
                temp1=4;
                break; 
            case "Green":
                temp1=5;
                break;
            case "Blue":
                temp1=6;
                break; 
            case "Voilet":
                temp1=7;
                break;
            case "Grey":
                temp1=8;
                break;
            case "White":
                temp1=9;
                break;    
        }
         switch (digit_band2_color){
            case "Black":
                temp2=0;
                break;
            case "Brown":
                temp2=1;
                break;
            case "Red":
                temp2=2;
                break;
            case "Orange":
                temp2=3;
                break; 
            case "Yellow":
                temp2=4;
                break; 
            case "Green":
                temp2=5;
                break;
            case "Blue":
                temp2=6;
                break; 
            case "Voilet":
                temp2=7;
                break;
            case "Grey":
                temp2=8;
                break;
            case "White":
                temp2=9;
                break;    
        }
          switch (multiplier_band3_color){
            case "Black":
                temp3=0;
                break;
            case "Brown":
                temp3=1;
                break;
            case "Red":
                temp3=2;
                break;
            case "Orange":
                temp3=3;
                break; 
            case "Yellow":
                temp3=4;
                break; 
            case "Green":
                temp3=5;
                break;
            case "Blue":
                temp3=6;
                break; 
            case "Voilet":
                temp3=7;
                break;
            case "Grey":
                temp3=8;
                break;
            case "White":
                temp3=9;
                break;    
        }
          switch (tolerance_band4_color){
            case "Brown":
                temp4=1;
                break;
            case "Red":
                temp3=2;
                break;
            case "Orange":
                temp4=0.05;
                break; 
            case "Yellow":
                temp4=0.02;
                break; 
            case "Green":
                temp4=0.5;
                break;
            case "Blue":
                temp4=0.25;
                break; 
            case "Voilet":
                temp4=0.1;
                break;
            case "Grey":
                temp4=0.01;
                break;
            case "Gold":
                temp4=5;
                break; 
            case "Silver":
                temp4=10;
                break;    
        }
        result=Math.pow(10,temp3);
        System.out.println("Resistance = "+temp1+temp2+result+"+-"+temp4+"%");     
    }
        public static void main(String[] args) {
        String a=JOptionPane.showInputDialog(null,"Please Enter Color in Proper Format like this Black,Brown etc");
        String b=JOptionPane.showInputDialog(null,"Please Enter Color in Proper Format like this Black,Brown etc");
        String c=JOptionPane.showInputDialog(null,"Please Enter Color in Proper Format like this Black,Brown etc");
        String d=JOptionPane.showInputDialog(null,"Please Enter Color in Proper Format like this Black,Brown etc");
        Resistance calculator=new Resistance(a,b,c,d);
}
    
}
