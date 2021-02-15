# tp-vigener
import java.util.Scanner;  
public class Main extends Cryptage {    
public static void main(String[] args)     {    
public class Cryptage {      
private static String uniformisation(String message)   {     
Scanner sc = new Scanner(System.in);        
System.out.print("Entrez votre message : \n\t");        
String message = sc.nextLine();        
System.out.print("Choisissez votre clef : \n\t");      
String clef = sc.nextLine();        
System.out.print("Message crypté : "+vigenere(message, clef));     }   }
for(int i = 33; i&lt;97;i++){message=message.replace(((char)i), ' ');}      
for(int i = 123;i&lt;127;i++){message=message.replace(((char)i), ' ');}  
message=message.replaceAll(" ","");
return message;     }         
public static String vigenere(String message, String clef)   
{String messageCrypte = ""; 
int compteur = 0; 
final char vigenereUn[] = {'a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z'};
char vigenereDeux[] = new char[26]; 
boolean rep = false;     
for(int i = 0; i&lt;clef.length();i++)             if(clef.charAt(i)!=' ') 
rep=true;                   
if(rep==false || clef==null)or(int i=0; i&lt;message.length(); i++) 
{                
int j=(int)(Math.random()*25+1); 
clef+=vigenereUn[j];             } 
System.out.println("Clef générée : "+clef+"\n");         }
message=uniformisation(message);  if(clef.length()&lt; message.length()) 
for(int i=clef.length(); i&lt;message.length(); i++)  
clef+=clef.charAt(i%clef.length());  while(compteur&lt;message.length())         { 
for(int i=0; i&lt;26; i++)                 if(clef.charAt(compteur)==vigenereUn[i])    
{    vigenereDeux[0]=vigenereUn[i];  int j=0;         for(int k=1; k&lt;26; k++)   { 
vigenereDeux[k]=(char)(vigenereDeux[0]+k);
if(vigenereDeux[k]>'z')   {    
vigenereDeux[k]=vigenereUn[0+j];   j++;    }    }
j=vigenereUn.length;    }  
for (int i=0; i&lt;26; i++) 
if(message.charAt(compteur)==vigenereUn[i])     {   
messageCrypte+=vigenereDeux[i];    i=vigenereUn.length;     }  
compteur++;}return messageCrypte; 
}     }

