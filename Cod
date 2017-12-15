

#include "LedControl.h" //  need the library
#include <time.h>
LedControl lc=LedControl(12,11,10,1); // 

  // pin 12 is connected to the MAX7219 pin 1
  // pin 11 is connected to the CLK pin 13
  // pin 10 is connected to LOAD pin 12
  // 1 as we are only using 1 MAX7219
  const int buttonPin = 9; 
  int buttonState = 0;
  
  int valx=0, valy=0; 
  int col=4, row=1;
  int ok=0;
  int pinx=A0, piny=A1;
  int button=7;
  int i=2;
  int coloana;
  
  
  int activare_tragere=0;
  int k=1;
  int kvar=0;
  int level=0;
  unsigned long previousMillis = 0; 
  unsigned long previousMillis_inamic = 0; 
  unsigned long previousMillis_inamic2 = 0; 
  const long interval1 = 200; 
  const long interval2 = 900;
  const long interval3 = 500; 
  int inamic=0;
  int n=7;
  int matrice[10][10];
  int random_col=0;
  int coloana_inamic;
  int coloana_inamic2;
  int random_col2=0;
  int eliminat2=0;
  int kvar2=0;
  int n2=7;
  int vieti=3;

  void afisare_level1() 
  {
  
      lc.setLed(0,4,2,true);
      lc.setLed(0,3,4,true);
      lc.setLed(0,4,3,true);
      lc.setLed(0,4,4,true);
      lc.setLed(0,4,5, true);
      lc.setLed(0,3,2, true);
      lc.setLed(0,5,2, true);
      
      delay(4000);
     
      lc.setLed(0,4,2,false);
      lc.setLed(0,3,4,false);
      lc.setLed(0,4,3,false);
      lc.setLed(0,4,4,false);
      lc.setLed(0,4,5, false);
      lc.setLed(0,3,2, false);
      lc.setLed(0,5,2, false);
    
      delay(1000);
    
  }


  void afisare_level2()
  {
        
      for(int i=0; i<=7; i++)
        for(int j=0; j<=7; j++)
          lc.setLed(0,i,j, false);
        
      lc.setLed(0,3,5,true);
      lc.setLed(0,4,5,true);
      lc.setLed(0,4,4, true);
      lc.setLed(0,4,3, true);
      lc.setLed(0,3,3, true);
      lc.setLed(0,3,2, true);
      lc.setLed(0,4,2, true);
      lc.setLed(0,5,2, true);
      
      delay(4000);
      
      lc.setLed(0,3,5,false);
      lc.setLed(0,4,5,false);
      lc.setLed(0,4,4, false);
      lc.setLed(0,4,3, false);
      lc.setLed(0,3,3, false);
      lc.setLed(0,3,2, false);
      lc.setLed(0,4,2, false);
      lc.setLed(0,5,2, false);
    
      delay(1000);
        
  }


   void afisare_level3(){
        
    for(int i=0; i<=7; i++)
      for(int j=0; j<=7; j++)
        lc.setLed(0,i,j, false);
        
      lc.setLed(0,2,6,true);
      lc.setLed(0,3,6,true);
      lc.setLed(0,4,6, true);
      lc.setLed(0,5,6, true);
      lc.setLed(0,5,5, true);
      lc.setLed(0,5,4, true);
      lc.setLed(0,3,4, true);
      lc.setLed(0,4,4, true);
      lc.setLed(0,5,4, true);
      lc.setLed(0,5,3, true);
      lc.setLed(0,5,2, true);
      lc.setLed(0,5,1, true);
      lc.setLed(0,4,1, true);
      lc.setLed(0,3,1, true);
      lc.setLed(0,2,1, true);
      delay(4000);
      
      for(int i=0; i<=7; i++)
        for(int j=0; j<=7; j++)
          lc.setLed(0,i,j, false);
    
      delay(1000);
           
  }

  
  int afisare_vieti()
  {
    
    if(vieti==3)
    {
             for(int i=0; i<=7; i++)
              for(int j=0; j<=7; j++)
                lc.setLed(0,i,j, false);
                
             lc.setLed(0,1,7,true);
             lc.setLed(0,2,6,true);
             lc.setLed(0,3,7,true);
       
             lc.setLed(0,4,7,true);
             lc.setLed(0,5,6,true);
             lc.setLed(0,6,7,true);
        
             lc.setLed(0,0,3,true);
             lc.setLed(0,0,4,true);
             lc.setLed(0,1,3,true);
             lc.setLed(0,1,4,true);
        
             lc.setLed(0,3,3,true);
             lc.setLed(0,3,4,true);
             lc.setLed(0,4,3,true);
             lc.setLed(0,4,4,true);
                  
             lc.setLed(0,6,3,true);
             lc.setLed(0,6,4,true);
             lc.setLed(0,7,3,true);
             lc.setLed(0,7,4,true);
                 
             delay(5000);
          
             for(int i=0; i<=7; i++)
               for(int j=0; j<=7; j++)
                 lc.setLed(0,i,j, false);
      }

      if(vieti==2)
      {
             for(int i=0; i<=7; i++)
              for(int j=0; j<=7; j++)
                lc.setLed(0,i,j, false);
                
             lc.setLed(0,1,7,true);
             lc.setLed(0,2,6,true);
             lc.setLed(0,3,7,true);
    
             lc.setLed(0,4,7,true);
             lc.setLed(0,5,6,true);
             lc.setLed(0,6,7,true);
    
             lc.setLed(0,0,3,true);
             lc.setLed(0,0,4,true);
             lc.setLed(0,1,3,true);
             lc.setLed(0,1,4,true);
    
             lc.setLed(0,3,3,true);
             lc.setLed(0,3,4,true);
             lc.setLed(0,4,3,true);
             lc.setLed(0,4,4,true);
              
        
             delay(5000);
      
             for(int i=0; i<=7; i++)
               for(int j=0; j<=7; j++)
                 lc.setLed(0,i,j, false);  
       }

     if(vieti==1)
     {
  
             for(int i=0; i<=7; i++)
              for(int j=0; j<=7; j++)
                lc.setLed(0,i,j, false);
            
             lc.setLed(0,1,7,true);
             lc.setLed(0,2,6,true);
             lc.setLed(0,3,7,true);
    
             lc.setLed(0,4,7,true);
             lc.setLed(0,5,6,true);
             lc.setLed(0,6,7,true);
    
             lc.setLed(0,0,3,true);
             lc.setLed(0,0,4,true);
             lc.setLed(0,1,3,true);
             lc.setLed(0,1,4,true);
    
           
             
             delay(5000);
      
            for(int i=0; i<=7; i++)
              for(int j=0; j<=7; j++)
                lc.setLed(0,i,j, false);
              
       }

  }

  void afisare_joc_castigat()  // am folosit delay pentru ca jocul e in pauza si nu deranjeaza activitatea
  {
      //sterge ecran
       for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);

//afiseaza litera W
       delay(100);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,1,i,true);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,6,i,true);
       lc.setLed(0,2,2,true);
       lc.setLed(0,3,3,true);
       lc.setLed(0,4,3,true);
       lc.setLed(0,5,2,true);

       delay(1000);

       
       //sterge ecran
       for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);
             
//afiseaza litera I
       delay(100);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,3,i,true);
       lc.setLed(0,2,6,true);
       lc.setLed(0,4,6,true);
       lc.setLed(0,2,1,true);
       lc.setLed(0,4,1,true);
       
       delay(1000);

      //sterge ecran
       for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);
             
//afiseaza litera N
       delay(100);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,1,i,true);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,6,i,true);
       for(int i=2; i<=5; i++) 
          for(int j=2; j<=5; j++) 
              if(i+j==7)
                  lc.setLed(0,j,i,true);
    
       delay(1000);

        for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);

 //afiseaza litera N
       delay(100);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,1,i,true);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,6,i,true);
       for(int i=2; i<=5; i++) 
          for(int j=2; j<=5; j++) 
              if(i+j==7)
                  lc.setLed(0,j,i,true);
    
       delay(1000);

       for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);

// afiseaza litera E
       delay(100);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,1,i,true);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,i,1,true);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,i,3,true);
       for(int i=1; i<=6; i++) 
          lc.setLed(0,i,6,true);
  
       delay(1000);

       for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);
             
// afiseaza litera R
       delay(100);
       for(int i=1; i<=5; i++) 
          lc.setLed(0,1,i,true);
       
       for(int i=1; i<=5; i++) 
          lc.setLed(0,i,6,true);

       for(int i=1; i<=5; i++) 
          lc.setLed(0,i,3,true);
      // for(int i=1; i<=5; i++) 
        //  lc.setLed(0,i,4,true);
      
       lc.setLed(0,5,5,true);
       lc.setLed(0,5,4,true);
       lc.setLed(0,3,2,true);
       lc.setLed(0,4,1,true);
       lc.setLed(0,5,1,true);
    

       delay(1000);

        for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
             lc.setLed(0,i,j, false);
    
        
  } 

  void afisare_game_over(){
  
        for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
            lc.setLed(0,i,j, false);
     
        for(int i=0; i<=7; i++)
           lc.setLed(0,i,7, true);
    
    
        for(int i=0; i<=7; i++)
           lc.setLed(0,i,0, true);
      
        for(int i=2; i<=5; i++)
           lc.setLed(0,1,i, true);
        for(int i=2; i<=5; i++)
           lc.setLed(0,3,i, true);

        lc.setLed(0,2,2, true);
        lc.setLed(0,2,5, true);
    
        lc.setLed(0,4,4, true);
        lc.setLed(0,5,3, true);
        lc.setLed(0,6,4, true);

        delay(10000);
        
         for(int i=0; i<=7; i++)
          for(int j=0; j<=7; j++)
            lc.setLed(0,i,j, false);
    
  }




            
int acelerare_tragere=0;

void functie_tragere(){ 
  
      unsigned long currentMillis = millis();
      if(k==3) 
      {
            lc.setLed(0, coloana, i-2, false); 
            k=2;  
      }
       
       
       while (currentMillis - previousMillis >= interval1-acelerare_tragere) 
       { 
                      previousMillis = currentMillis; 
                      k++;   
                      lc.setLed(0, coloana, i, true);
                      matrice[i][coloana]=1; 
                      i++;
 
       }
       
       if(i>7)
       { 
               lc.setLed(0, coloana, i-2, false); 
               lc.setLed(0, coloana, i-1, false); 
               
               i=2; 
               activare_tragere=0;
               k=1; 
       }
             
  }







 int eliminat=0;
 int alege_coloana=0;

 
void mutare_inamic_tip1(){

      unsigned long currentMillis = millis();
      if((inamic==0 || inamic==1 || inamic==2) && alege_coloana==0)
      {
           alege_coloana=1;
           coloana_inamic=rand()%8;  
           for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic]=0;
      }
      
       
      if(kvar==2)
      {  
            lc.setLed(0, coloana_inamic, n+2, false);
            kvar=1;
      }
         
      while (currentMillis - previousMillis_inamic >= interval2) 
      { 
                  previousMillis_inamic = currentMillis; 
                  kvar++;
                  
                  if(matrice[n][coloana_inamic]==1 )
                  {
                      eliminat=1;   
                      n=-1;
                      for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana]=0;    
                  }
                    
                  if(eliminat==0)
                  {
                      lc.setLed(0, coloana_inamic, n, true); //matrice[n][coloana_inamic]=2;
                  }
                  
                  n--;
       }
       
       if(n<0)
       { 
                 if(eliminat==0) 
                 {
                    lc.setLed(0, coloana_inamic, n+2, false); 
                    lc.setLed(0, coloana_inamic, n+1, false); 
                    vieti--;  
                 } 
                 n=7; 
                 inamic++;
                 kvar=1;
                 eliminat=0;
                 alege_coloana=0;
        }
        
   }


int j=1;

void mutare_inamic_tip2(){
    
      unsigned long currentMillis = millis();
      if(inamic==3 && alege_coloana==0) 
      {
          coloana_inamic2=3;
          alege_coloana=1;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic2]=0;
      }
      if(inamic==4&& alege_coloana==0)
      {
           coloana_inamic2=5;
           alege_coloana=1;
           for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic2]=0;
      }
      if(inamic==5 &&alege_coloana==0)
      {
          coloana_inamic2=1;
          alege_coloana=1;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic2]=0;
      }
       
      if(kvar2==2)
      {
            lc.setLed(0, coloana_inamic2, n2+2, false); kvar2=1;
      }
      
      while (currentMillis - previousMillis_inamic2 >= interval3)  // fuge mai repede
      {
             previousMillis_inamic2 = currentMillis; 
             kvar2++;
             if(matrice[n2][coloana_inamic2]==1)
                    {
                        eliminat2=1;
                        for(int cont=1; cont<=7 ; cont++) 
                              matrice[cont][coloana]=0; n=-1;
                    }
             if(eliminat2==0)
                lc.setLed(0, coloana_inamic2, n2, true);
                n2--;
      }
      
      if(n2<0)
      {
             if(eliminat2==0) {lc.setLed(0, coloana_inamic2, n2+2, false); lc.setLed(0, coloana_inamic2, n2+1, false); vieti--;}  
             n2=7;
             inamic++;
             kvar2=1;
             eliminat2=0; 
             alege_coloana=0;
      }
  
  }
  


  int urma_inamic[100]={1,1,1};
  int previousMillis_inamici[100]; 
  int coloana_inamici[100] ;
  
  int eliminat1_doua=0;
  int eliminat2_doua=0;
  int coloana_inamic_doua;
  int p=1;

void mutare_inamic_doua(){

      unsigned long currentMillis = millis();
      if(inamic==7 &&alege_coloana==0)
      {
         alege_coloana=1;
         coloana_inamic_doua=3; 
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua]=0;
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua+1]=0;
      }
         
      if(inamic==8 && alege_coloana==0)
      {
         coloana_inamic_doua=1;
         alege_coloana=1; 
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua]=0;
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua+1]=0;  
      }
      if(inamic==9 && alege_coloana==0)
      {
         coloana_inamic_doua=6;
         alege_coloana=1; 
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua]=0;
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua+1]=0;
         p=2;
         acelerare_tragere=50;
      }  
      if(inamic==10 && alege_coloana==0)
      {
         coloana_inamic_doua=4;
         alege_coloana=1; 
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua]=0;
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua+1]=0;
         p=2;
         acelerare_tragere=50;
      }   
      if(inamic==11 && alege_coloana==0)
      {
         coloana_inamic_doua=0;
         alege_coloana=1; 
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua]=0;
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua+1]=0;
         p=2;
         acelerare_tragere=50;
      }   
       
      if(inamic==12 && alege_coloana==0)
      {
         coloana_inamic_doua=0;
         alege_coloana=1; 
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua]=0;
         for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic_doua+1]=0;
         p=2;
         acelerare_tragere=40;
      }    
              
      if(kvar2==2)
      {
          lc.setLed(0, coloana_inamic_doua, n2+2, false); 
          lc.setLed(0, coloana_inamic_doua+1, n2+2, false); 
          kvar2=1;
      }
       
       while (currentMillis - previousMillis_inamic2 >= interval2/p)  
       {
             previousMillis_inamic2 = currentMillis; 
             kvar2++;
         
             if(matrice[n2][coloana_inamic_doua]==1)
             {
                       eliminat1_doua=1; 
                       for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana]=0;
             }
                  
             if(matrice[n2][coloana_inamic_doua+1]==1)
             {
                      eliminat2_doua=1; 
                      for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana]=0;
             }
                    
             if(eliminat1_doua==0 && eliminat2_doua==0)
             {
                     lc.setLed(0, coloana_inamic_doua, n2, true);
                     lc.setLed(0, coloana_inamic_doua+1, n2, true);
             }
                   
             if(eliminat1_doua==0 && eliminat2_doua!=0)
                    lc.setLed(0, coloana_inamic_doua, n2, true);
                    
             if(eliminat1_doua!=0 && eliminat2_doua==0)
                    lc.setLed(0, coloana_inamic_doua+1, n2, true);
             
             n2--;
        }
           
        if(n2<0)
        { 
              if(eliminat1_doua==0) 
              {
                  lc.setLed(0, coloana_inamic_doua, n2+2, false); 
                  lc.setLed(0, coloana_inamic_doua, n2+1, false);  
                  vieti--;
              } 
              
             if(eliminat2_doua==0) 
             {
                  lc.setLed(0, coloana_inamic_doua+1, n2+2, false); 
                  lc.setLed(0, coloana_inamic_doua+1, n2+1, false); 
                  vieti--;
             }
             
             n2=7;
              
             inamic++;
             kvar2=1;
             alege_coloana=0;
             eliminat1_doua=0; 
             eliminat2_doua=0;
        }
  }

  

int coloana_inamic3;
int interval4=700;
int accel=0;
int oke=0;

void mutare_inamic_tip3(){
  
      unsigned long currentMillis = millis();
      
      if(inamic==14 && alege_coloana==0)
      {
          coloana_inamic3=3;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic3]=0;
          alege_coloana=1;
      }
      
      if(inamic==15 && alege_coloana==0)
      {
          coloana_inamic3=1;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic3]=0;
          accel=200;
          alege_coloana=1;
      }
    
      if(inamic==16 && alege_coloana==0)
      {
          coloana_inamic3=5;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic3]=0;
          accel=250;
          acelerare_tragere=100;
          alege_coloana=1;
      }
      
      if(inamic==17 && alege_coloana==0)
      {
          accel=400;
          coloana_inamic3=2;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic3]=0;
          alege_coloana=1;
      }
      
      if(inamic==18 && alege_coloana==0)
      {
          accel=400;
          coloana_inamic3=4;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic3]=0;
          alege_coloana=1;
      }
    
      if(inamic==19 && alege_coloana==0)
      {
          accel=500;
          coloana_inamic3=1;
          for(int cont=1; cont<=7 ; cont++) matrice[cont][coloana_inamic3]=0;
          alege_coloana=1;
      }
         
      if(kvar2==2)
      {
            lc.setLed(0, coloana_inamic3, n2+2, false); 
            lc.setLed(0, coloana_inamic3-1, n2+2, false);  
            lc.setLed(0, coloana_inamic3+1, n2+2, false);
            kvar2=1;
      }
      
      
      while (currentMillis - previousMillis_inamic2 >= interval4-accel) 
      { 
            previousMillis_inamic2 = currentMillis; 
            kvar2++;
            if(matrice[n2][coloana_inamic3]==1)
            {
                eliminat2=1; 
                for(int cont=7; cont>=2; cont--)
                       lc.setLed(0, coloana_inamic3, cont, false); 
                for(int cont=1; cont<=7 ; cont++) 
                       matrice[cont][coloana]=0;
            }
                  
            if(eliminat2==0)
            {
                 lc.setLed(0, coloana_inamic3, n2, true); 
                 lc.setLed(0, coloana_inamic3-1, n2, true); 
                 lc.setLed(0, coloana_inamic3+1, n2, true); }
                 n2--;
            }
            
            if(n2<0)
            { 
                if(eliminat2==0) 
                {   lc.setLed(0, coloana_inamic3, n2+2, false);
                    lc.setLed(0, coloana_inamic3-1, n2+2, false); 
                    lc.setLed(0, coloana_inamic3+1, n2+2, false); 
                    lc.setLed(0, coloana_inamic3, n2+1, false); 
                    lc.setLed(0, coloana_inamic3-1, n2+1, false);
                    lc.setLed(0, coloana_inamic3+1, n2+1, false);
                     vieti=vieti-3; 
                 }  
               
               n2=7;
               inamic++;
               kvar2=1;
               eliminat2=0; 
               alege_coloana=0;
            }
 
  }


 

  int joc=0;
  int timp=0;


  void setup()
  {
      
      lc.shutdown(0,false);// turn off power saving, enables display
      lc.setIntensity(0,8);// sets brightness (0~15 possible values)
      lc.clearDisplay(0);// clear screen
      pinMode(pinx,INPUT);
      pinMode(piny, INPUT);
      pinMode(buttonPin, INPUT);
      Serial.begin(9600);       
  }
  
  
  int prevMillis=0;
  int jocMillis=0;
  int contor_buton=0;
  


 void loop(){
  
     unsigned long currentMillis = millis();
    
     buttonState = digitalRead(buttonPin);
      
     valx=analogRead(pinx);
     valy=analogRead(piny);
  
     valx=map(valx,0,1024,0,7);
     valy=map(valy,0,1024,0,7);

     if(timp==0)
      {
        timp=1;
        srand(time(NULL));
        }
  
    if(buttonState==1&&joc==0 )
       joc=1; 

   /*
    if(buttonState==1&&joc==1 && oke==0)
      {
      contor_buton++;
      if(contor_buton>5)
          {
      for(int i=0; i<=7; i++)
      for(int j=0; j<=7; j++)
        lc.setLed(0,i,j, false);
        
          joc=0; 
          vieti=3;
          level=0;
          inamic=0; 
          oke=1;
          delay(1000);
          }
      }

      */
   
    
   
     
   if(joc==1)   
     
      {
              //if(currentMillis-prevMillis>=150){
       
            if(valx<3 )
                      if(col==0)
                      {  
                            lc.setLed(0,col,row,false);
                            col=7;
                            lc.setLed(0, col, row, true);
                            //prevMillis=currentMillis;
                            delay(150);
                      }
                        
                      else
                      {
                        if(col!=0)
                            lc.setLed(0,col,row,false);
                            col=col-1;
                            lc.setLed(0, col, row, true);
                            //prevMillis=currentMillis;
                             delay(150);
                      }
             else
             if(valx>3)
                      if(col==7)
                      {
                          col=1;
                          lc.setLed(0, col, row, true);
                          lc.setLed(0,7,row,false);
                         // prevMillis=currentMillis;
                          delay(150);
                       }
                      else
                      {
                          lc.setLed(0,col,row,false);
                          col=col+1;
                          lc.setLed(0, col, row, true);
                          //prevMillis=currentMillis;
                           delay(150);
                      }
                         
             if(valy<3 && valx==3 && activare_tragere==0 )
              {
                activare_tragere=1;
                coloana=col;
              }
            
             if(activare_tragere==1)
              functie_tragere();
               
             
             if(level==0)   // pentru level de inceput
             {
                level=1;
                afisare_level1();
                afisare_vieti();
                delay(500);
                lc.setLed(0,col,row,true);
             }
          
            if(inamic==0 )
               mutare_inamic_tip1(); 
      
            if(inamic==1)
               mutare_inamic_tip1(); 
      
            if(inamic==2 )
              mutare_inamic_tip1(); 
      
            if(inamic==3)
                mutare_inamic_tip2(); 
                
            if(inamic==4)
                mutare_inamic_tip2(); 
            
            if(inamic==5)
                mutare_inamic_tip2(); 
  
            if(inamic==6 ) // fals inamic - pentru a trece la level2
            {
                level=2;
                inamic++;
            }
            
            if(level==2 && vieti!=0) 
            {
                level=-1;
                afisare_level2();
                afisare_vieti();
                delay(500);
                lc.setLed(0,col,row,true);
            }
      
           
            if(inamic==7)
              mutare_inamic_doua();
  
            if(inamic==8)
              mutare_inamic_doua();
  
            if(inamic==9)
              mutare_inamic_doua();
  
            if(inamic==10)
              mutare_inamic_doua();
  
            if(inamic==11)
              mutare_inamic_doua();
            
            if(inamic==12)
              mutare_inamic_doua();
  
            if(inamic==13) // fals inamic 
            {
                level=3;
                inamic++;
            }
  
            if(level==3 && vieti!=0)
            {
              
                level=-1;
                afisare_level3();
                afisare_vieti();
                delay(500);
                lc.setLed(0,col,row,true);
               
            }
  
           if(inamic==14)        
             mutare_inamic_tip3();
  
           if(inamic==15)  
                mutare_inamic_tip3();  
                
           if(inamic==16)  
                mutare_inamic_tip3(); 
  
           if(inamic==17)  
                mutare_inamic_tip3(); 
                
           if(inamic==18)  
                mutare_inamic_tip3();
                
           if(inamic==19)  
                mutare_inamic_tip3(); 
                
           if(inamic==20) // fals inamic
           {    
                joc=0;
                level=0;
                afisare_joc_castigat();
                vieti=3;
                inamic=0;
           }
           
           if(vieti==0)
           {
                afisare_game_over();
                joc=0;
                vieti=3;
                level=0;
                inamic=0;
           }
  
     
      } // acolada care incadreaza joc=1
      
  
   
       
 }




