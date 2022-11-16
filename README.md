# -5
Страница 195 номер 18

 В тексте определить все согласные буквы, встречающиеся не более чем в двух словах.
 

import java.util.ArrayList;

import java.util.Scanner;


public class Test {


        public static void main(String args[]){
        
            String str = new String("Тестоваястрока!");
            
            Scanner scan = new Scanner(System.in);
            
System.out.println("Введите строку дял проверки гласных букв: ");

str =  scan.nextLine();

            String tmp1;
            
            String tmp2;
            
            int VowelsSound =0;
            

ArrayList<Character>arr = new ArrayList<Character>();

arr.add('а');

arr.add('е');

arr.add('ё');

arr.add('и');

arr.add('о');

arr.add('у');

arr.add('ы');

arr.add('э');

arr.add('ю');

arr.add('я');

for(int i=0; i<=arr.size()-1; i++){

                tmp2=String.valueOf(arr.get(i));
                
for(int j =0 ; j<=str.length()-1; j++){

                    tmp1=String.valueOf(str.charAt(j));
                    
if(tmp2.equals(tmp1))

VowelsSound++;
                }
                
            }
            
System.out.println("Встроке "+VowelsSound+" гласныхбукв!"); 

}

}
