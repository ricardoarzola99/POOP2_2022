# POOP2_2022
Práctica correspondiente a sintaxis de lenguaje con el entorno Java


package POOP2;
public class POOP2 {
    public static void main(String[] args) {
        
        // TODO code application logic here
        System.out.println("Hola Mundo");
     KeyboardInput teclado= new KeyboardInput();
     KeyboardInput in=new KeyboardInput();
     int word=0;
        System.out.println("---------IF-----------");
        System.out.println("Ingrese el valor de A:");
        int a=teclado.readInteger();
        System.out.println("Ingrese valor de B:");
        int b=teclado.readInteger();
        if (a<b) {
            System.out.println("A es menor que B");
            } else {
            System.out.println("A es mayor o igual a B");
        }
       
             System.out.println("---------IF 2-----------");
        if (a<=b) {
            System.out.println("A es menor o igual que B");
            } else {
            System.out.println("A es mayor que B");
        } 
        
        System.out.println("---------IF FUNCION-----------");
        if (f(a,b)){
            System.out.println("A es menor que b");
            }else{
            System.out.println("A es mayor o igual que b");
        }
        
    System.out.println("---------SWITCH-----------");
        System.out.println("Ingrese un día de la semana en número:");
    int dia=teclado.readInteger();
        switch (dia) {
            case 1:System.out.println("Domingo");break;
            case 2:System.out.println("Lunes");break;
            case 3:System.out.println("Martes");break;
            case 4:System.out.println("Miércoles");break;
            case 5:System.out.println("Jueves");break;
            case 6:System.out.println("Viernes");break;
            case 7:System.out.println("Sábado");break;
            default:
                System.out.println(dia+ "No es un día de la semana");
        }
        
        System.out.println("---------SWITCH 2-----------");
        System.out.println("Ingrese una vocal:");
    char letra=teclado.readCharacter(); 
        switch (letra) {
            case 'a':System.out.println("Se escribió a ");break;
            case 'e':System.out.println("Se escribió e ");break;
            case 'i':System.out.println("Se escribió i ");break;
            case 'o':System.out.println("Se escribió o ");break;
            case 'u':System.out.println("Se escribió u ");break;
            default:
                System.out.println("No se escribió ninguna vocal");
        }
    
     
         System.out.println("---------SWITCH con while-----------");
         do {            
        System.out.println("Opción 1: letra a");
        System.out.println("Opción 2: letra b");
        System.out.println("Opción 3: letra c");
        System.out.println("Opción 4: letra d");
        System.out.println("Opción 5: letra e");
        System.out.println("Opción 6: letra f");
        System.out.println("Opción 7: Salir");
        System.out.println("Digite una opción: ");
        word=teclado.readInteger();
        switch (word) {
            case 1:System.out.println("Se escribió a ");break;
            case 2:System.out.println("Se escribió b ");break;
            case 3:System.out.println("Se escribió c ");break;
            case 4:System.out.println("Se escribió d ");break;
            case 5:System.out.println("Se escribió e ");break;
            case 6:System.out.println("Se escribió f ");break;
            default:
                System.out.println("No se escribió una letra válida");
                break;} 
        } while (word!=7);
  System.out.println("---------FOR ASCENDIENTE-----------");  
        for (int i = 0; i < 10; i++) {
            System.out.println(i);      
        }
 System.out.println("---------FOR DESCENDIENTE-----------");  
        for (int i = 10; i > 0; i--) {
            System.out.println(i);    
        }
 
 System.out.println("---------FOR CON ARREGLO-----------");
int[] arreglo=new int [10];
        System.out.println("Valores iniciales del arreglo");
        for (int j = 0; j < arreglo.length; j++) {//Almacena la informaciòn del arreglo
            System.out.println("El arreglo es ["+j+"]:"+arreglo[j]);
            }
        System.out.println("Ingresando valores al arreglo");
                for (int j = 0; j < arreglo.length; j++) {//Almacena la informaciòn del arreglo
            arreglo[j]=j*10;
            }
                System.out.println("Valores finales del arreglo");
        for (int j = 0; j < arreglo.length; j++) {//Lee la informaciòn del arreglo
            System.out.println("El arreglo es ["+j+"]:"+arreglo[j]);
        }
 System.out.println("---------FOR CON IF ANIDADO-----------");
for (int i=0; i< 10; i++){
System.out.print("Escriba un digito: ");
 int n;
            n = in.readInteger();
if(n==0){
    System.out.println("Division entre cero.");
continue;
}
System.out.println("100/" + n +" =" + 100.0/n);      
 }
    
System.out.println("---------WHILE CON IF-----------");
while (true) {
System.out.print("Escriba un digito: ");
int n = in. readInteger();
if (n==5) {
System.out.println("Escribio un 5. Termina");
break; }}

System.out.println("---------DO WHILE-----------");
int n = 0; 
do {
System.out.println("Contando hacia arriba" + n);
n++;
} while (n == 10 );
do {
System.out.println("Contando hacia abajo " + n); n--;
} while (n > 0); 
 System.out.println("El menor de 5 y 8 es: " + min(5,8));
    }  
    
public static boolean f(int x, int y){
        return x<y;
        }
private static int min (int a, int b) {
if (a < b){ return a;}
else return b;} }
