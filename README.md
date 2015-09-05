# Game-Fight
#include <stdio.h>
#include <windows.h>
void espacios (int n);
void main ()
{
while(1)
{
srand(time(NULL));

system("color 0F");
char player1[100]={"player1"},player2[100]={"player2"},arma1,arma2;
float player1vida=10000,player2vida=10000,golpeplayer1,golpeplayer2;
int CAR1=5,FUE1=5,INT1=5,DES1=10,atributoponer1=0,tipoarma1,tipogolpe1;//Player1
int CAR2=10,FUE2=5,INT2=5,DES2=5,atributoponer2=0,tipoarma2,tipogolpe2;//Player2


printf("Iniciamos el PVP: Inserte nombre para el player1 \n");
           	gets(player1);
printf("Inserte nombre para el player2\n");
           	gets(player2);
printf("Ahora se¤or %s le toca ponerle los atributos de PVP,\n <Se te asigna por defecto 1 punto en cada atributo>\n",player1);

            	printf("Tienes 10 puntos de atributo. Elige sabiamente entre Carisma, Fuerza, Inteligencia, Destreza\n");
                        while(atributoponer1==0)
                        {
                        	printf("Carisma: ");scanf("%d",&CAR1);
                           CAR1++;
                           printf("Fuerza: ");scanf("%d",&FUE1);
                           FUE1++;
                           printf("Inteligencia: ");scanf("%d",&INT1);
                           INT1++;
                           printf("Destreza: ");scanf("%d",&DES1);
                           DES1++;
                        if((CAR1+INT1+FUE1+DES1)==14)
                        	atributoponer1=1;
                        else
                          	printf("ERROR: Has puesto mas o menos de 10 puntos de atributos\n");
                        }
                        system("pause");




printf("Se¤or  ,%s le toca elegir el tipo de arma que va a usar:\n",player1);
printf("1-Espada");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+5");espacios(5);printf("Fuerza: +2");espacios(5);printf("Inteligencia:-2\n");
printf("2-Arco");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+5");espacios(5);printf("Destreza: +2");espacios(5);printf("Inteligencia:+1");espacios(5);printf("Fuerza:-1\n");
printf("3-Mazo");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+8");espacios(5);printf("Destreza: -2");espacios(5);printf("Inteligencia:-2");espacios(5);printf("Fuerza:+1\n");
printf("4-Escudo");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+2");espacios(5);printf("Destreza: +5");espacios(5);printf("Inteligencia:+1\n");
scanf("%d",&tipoarma1);

	while(tipoarma1!=1&&tipoarma1!=2&&tipoarma1!=3&&tipoarma1!=4)
   	{
   	printf("ERROR: Introduce un valor valido: ");
      scanf("%d",&tipoarma1);
		}
   switch(tipoarma1)
   	{
      	case 1:
         arma1=5,FUE1+=2,INT1-=2;
         break;
         case 2:
         arma1=5,DES1+=2,INT1+=1,FUE1-=1;
         break;
         case 3:
         arma1=8,FUE1+=2,DES1-=2,INT1-=2,FUE1+=1;
         break;
         case 4:
         arma1=2,DES1+=5,INT1+=1;
         break;
      }

      printf("Tus atributos han quedado asi:\n1-Carisma: %d\n2-Fuerza: %d\n3-Inteligencia: %d\n4-Destreza: %d\n",CAR1,FUE1,INT1,DES1);
            		system("\npause");
               	system("cls");

      printf("Ahora se¤or %s le toca ponerle los atributos de PVP,\n <Se te asigna por defecto 1 punto en cada atributo>\n",player2);
				printf("Tienes 10 puntos de atributo. Elige sabiamente entre Carisma, Fuerza, Inteligencia, Destreza\n");
                        while(atributoponer2==0)
                        {
                        	printf("Carisma: ");scanf("%d",&CAR2);
                           CAR2++;
                           printf("Fuerza: ");scanf("%d",&FUE2);
                           FUE2++;
                           printf("Inteligencia: ");scanf("%d",&INT2);
                           INT2++;
                           printf("Destreza: ");scanf("%d",&DES2);
                           DES2++;
                        if((CAR2+INT2+FUE2+DES2)==14)
                        	atributoponer2=1;
                        else
                          	printf("ERROR: Has puesto mas o menos de 10 puntos de atributos\n");
                        }
                        system("pause");


printf("Se¤or  ,%s le toca elegir el tipo de arma que va a usar:\n",player2);
printf("1-Espada");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+5");espacios(5);printf("Fuerza: +2");espacios(5);printf("Inteligencia:-2\n");
printf("2-Arco");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+5");espacios(5);printf("Destreza: +2");espacios(5);printf("Inteligencia:+1");espacios(5);printf("Fuerza:-1\n");
printf("3-Mazo");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+8");espacios(5);printf("Destreza: -2");espacios(5);printf("Inteligencia:-2");espacios(5);printf("Fuerza:+1\n");
printf("4-Escudo");espacios(3);printf("Caracteristicas:");espacios(5);printf("Da¤o:+2");espacios(5);printf("Destreza: +5");espacios(5);printf("Inteligencia:+1\n");
scanf("%d",&tipoarma2);
	while(tipoarma2!=1&&tipoarma2!=2&&tipoarma2!=3&&tipoarma2!=4)
   	{
   	printf("ERROR: Introduce un valor valido: ");
      scanf("%d",&tipoarma2);
		}
   switch(tipoarma2)
   	{
      	case 1:
         arma2=5,FUE2+=2,INT2-=2;
         break;
         case 2:
         arma2=5,DES2+=2,INT2+=1,FUE2-=1;
         break;
         case 3:
         arma2=8,FUE2+=2,DES2-=2,INT2-=2,FUE2+=1;
         break;
         case 4:
         arma2=2,DES2+=5,INT2+=1;
         break;
      }

      printf("Tus atributos han quedado asi:\n1-Carisma: %d\n2-Fuerza: %d\n3-Inteligencia: %d\n4-Destreza: %d\n",CAR2,FUE2,INT2,DES2);
            		system("pause");
               	system("cls");

	for(int i=1;player1vida>0&&player2vida>0;i++)//inicio del enfrentamiento PVP
	{//Inicio de cuenteo de rondas
   int cura1=0,cura2=0;
   float golpeplayer1,critico1=1,elusion1=0,puntosdecura1,GCritico1=0; //player1
   float golpeplayer2,critico2=1,elusion2=0,puntosdecura2,GCritico2=0; //player2
   int Posibilidadcritico1=rand()%100;Sleep(85);
   int Posibilidadelusion2=rand()%100;Sleep(212);
   float azar1=rand()%110+90;azar1=azar1/100;Sleep(145);
   int Posibilidadcritico2=rand()%100;Sleep(194);
   float azar2=rand()%110+90;azar2=azar2/100;Sleep(167);
   int Posibilidadelusion1=rand()%100;
      if(i%5==0)
         {
         system("cls");
         }

      if(i==1)
   	printf("Inicia el combate %s Vs %s\n\n",player1,player2);
      printf("\n\nInicia la  Ronda: %d\n",i);
      printf("Se¤or %s , eliga el tipo de golpe\n",player1);
      printf("1-Golpe normal\n2-Cura(Solo te curas a ti mismo)\n3-Critico(Critico mas potente,pero el normal mas bajo)\n4-Elusion aumentada (Tu golpe es mas flojo)\n");
      scanf("%d",&tipogolpe1);
      	while(tipogolpe1!=1&&tipogolpe1!=2&&tipogolpe1!=3&&tipogolpe1!=4)
         	{
             printf("ERROR al introducir numero, vuelva a introducirlo: ");
             scanf("%d",&tipogolpe1);
         	}
      	switch(tipogolpe1)
         	{
            	case 1:break;
               case 2:cura1=1;break;
               case 3:critico1+=2.5,FUE1-=2;break;
               case 4:Posibilidadelusion1+=25,FUE1-=2;break;
            }

      printf("Se¤or %s , eliga el tipo de golpe\n",player2);
      printf("1-Golpe normal\n2-Cura(Solo te curas a ti mismo)\n3-Critico(Critico mas potente, no mas posibilidad)\n4-Elusion aumentada (Tu golpe es mas flojo)\n");
      scanf("%d",&tipogolpe2);
      	while(tipogolpe2!=1&&tipogolpe2!=2&&tipogolpe2!=3&&tipogolpe2!=4)
         	{
             printf("ERROR al introducir numero, vuelva a introducirlo: ");
             scanf("%d",&tipogolpe2);
         	}
      	switch(tipogolpe2)
         	{
            	case 1:break;
               case 2:cura2=1;break;
               case 3:critico2+=2.5,FUE2-=2;break;
               case 4:Posibilidadelusion2+=25,FUE2-=2;break;
            }


      	if(CAR1>=2&&Posibilidadcritico1>75)//Criticos de player1
      	{
      		switch(CAR1)
              		{case 2:critico1+=0.5,GCritico1=1;break;case 3:critico1+=0.8,GCritico1=1;break;
                  case 4:critico1+=1.2,GCritico1=1;break;case 5:critico1+=1.7,GCritico1=1;break;
                  case 6:critico1+=2.1,GCritico1=1;break;case 7:critico1+=2.6,GCritico1=1;break;
                  case 8:critico1=3.1,GCritico1=1;break;case 9:critico1+=3.6,GCritico1=1;break;
                  default:critico1+=4,GCritico1=1;
                  }
      	}
         if(CAR2>=2&&Posibilidadcritico2>75)//Criticos de player2
      	{
      		switch(CAR2)
              		{case 2:critico2+=0.5,GCritico2=1;break;case 3:critico2+=1.8,GCritico2=1;break;
                  case 4:critico2+=1.2,GCritico2=1;break;case 5:critico2+=1.7,GCritico2=1;break;
                  case 6:critico2+=2.1,GCritico2=1;break;case 7:critico2+=2.6,GCritico2=1;break;
                  case 8:critico2+=3.1,GCritico2=1;break;case 9:critico2+=3.6,GCritico2=1;break;
                  default:critico2+=4;
                  }
      	}


          	if(DES1>=2)//Probabilidad de elusion de player1
          	{
            	switch(DES1)
            	{
               case 2:
               	if(Posibilidadelusion1>90)
                  elusion1=1;break;
               case 3:
               	if(Posibilidadelusion1>85)
                  elusion1=1;break;
               case 4:
               	if(Posibilidadelusion1>80)
                  elusion1=1;break;
               case 5:
               	if(Posibilidadelusion1>75)
                  elusion1=1;break;
               case 6:
               	if(Posibilidadelusion1>70)
                  elusion1=1;break;
               case 7:
               	if(Posibilidadelusion1>65)
                  elusion1=1;break;
               case 8:
               	if(Posibilidadelusion1>60)
                  elusion1=1;break;
               case 9:
               	if(Posibilidadelusion1>55)
                  elusion1=1;break;
               case 10:
               	if(Posibilidadelusion1>50)
                  elusion1=1;break;
               default:
               	if(Posibilidadelusion1>45)
                  elusion1=1;
            	}
            }//Fin Probabilidad de elusion de player1
          if(DES2>=2)//Probabilidad de elusion de player2
          	{
            	switch(DES2)
            	{
               case 2:
               	if(Posibilidadelusion1>90)
                  elusion2=1;break;
               case 3:
               	if(Posibilidadelusion1>85)
                  elusion2=1;break;
               case 4:
               	if(Posibilidadelusion1>80)
                  elusion2=1;break;
               case 5:
               	if(Posibilidadelusion1>75)
                  elusion2=1;break;
               case 6:
               	if(Posibilidadelusion1>70)
                  elusion2=1;break;
               case 7:
               	if(Posibilidadelusion1>65)
                  elusion2=1;break;
               case 8:
               	if(Posibilidadelusion1>60)
                  elusion2=1;break;
               case 9:
               	if(Posibilidadelusion1>55)
                  elusion2=1;break;
               case 10:
               	if(Posibilidadelusion1>50)
                  elusion2=1;break;
               default:
               	if(Posibilidadelusion1>45)
                  elusion2=1;
            	}
            }//Fin Probabilidad de elusion de player2
          if(cura1==1)
          	{
            puntosdecura1=INT1*3*azar1;
            }
          if(cura2==1)
          	{
            puntosdecura2=INT2*3*azar2;
            }
          //fin de probabilidades y formulas, ahora toca el daño entre ellos y las reaciones de los ataques
      if(tipogolpe1!=2&&tipogolpe2!=2)
          {
          	if(elusion1==0)
          	{

               if(GCritico1==0)
               	{
                  golpeplayer1=((FUE1+arma1)*azar1);
                  if(golpeplayer1<0)
                  	golpeplayer1=0;
          			player2vida-=golpeplayer1;
          			printf("\n%s da un golpe de:%g a %s\n",player1,golpeplayer1,player2);
            		printf("\nA %s le quedan %g puntos de vida\n",player2,player2vida);
                  }
               else
               	{
                  golpeplayer1=((FUE1+arma1)*azar1)*critico1;
                  if(golpeplayer1<0)
                  	golpeplayer1=0;
          			player2vida-=golpeplayer1;
                  printf("\n%s da un Critico de:%g a %s\n",player1,golpeplayer1,player2);
            		printf("\nA %s le quedan %g puntos de vida\n",player2,player2vida);
                  }
          	}
          	else
          		printf("\n%s intenta dar a %s pero ha eludido el golpe\n",player1,player2);
           	if(elusion2==0)
          	{

               if(GCritico2==0)
               {
               golpeplayer2=((FUE2+arma2)*azar2);
               if(golpeplayer2<0)
                  	golpeplayer2=0;
          		player1vida-=golpeplayer2;
          		printf("\n%s da un golpe de:%g a %s\n",player2,golpeplayer2,player1);
            	printf("\nA %s le quedan %g puntos de vida\n",player1,player1vida);
            	}
               else
               {
               golpeplayer2=((FUE2+arma2)*azar2)*critico2;
               if(golpeplayer2<0)
                  	golpeplayer2=0;
          		player1vida-=golpeplayer2;
          		printf("\n%s da un Critico de:%g a %s\n",player2,golpeplayer2,player1);
            	printf("\nA %s le quedan %g puntos de vida\n",player1,player1vida);
            	}
          	}
          	else
          		printf("\n%s intenta dar a %s pero ha eludido el golpe\n",player2,player1);

          }

      if(tipogolpe1==2&&tipogolpe2==2)
      	{
         player1vida=player1vida+puntosdecura1*critico1;
         player2vida=player2vida+puntosdecura2*critico2;
         printf("%s se cura %g puntos de vida\n",player1,puntosdecura1*critico1);
         printf("\nA %s le quedan %g puntos de vida\n",player1,player1vida);
         printf("%s se cura %g puntos de vida\n",player2,puntosdecura2*critico2);
         printf("\nA %s le quedan %g puntos de vida\n",player2,player2vida);
         }

      if(tipogolpe1==2&&tipogolpe2==1||tipogolpe1==2&&tipogolpe2==3||tipogolpe1==2&&tipogolpe2==4)
      	{
         	player1vida=player1vida+puntosdecura1*critico1;
            printf("%s se cura %g puntos de vida\n",player1,puntosdecura1*critico1);
            printf("\nA %s le quedan %g puntos de vida\n",player1,player1vida);
            if(elusion2==0)
          	{

               if(GCritico2==0)
               {
               golpeplayer2=((FUE2+arma2)*azar2);
               if(golpeplayer2<0)
                  	golpeplayer2=0;
          		player1vida-=golpeplayer2;
          		printf("\n%s da un golpe de:%g a %s\n",player2,golpeplayer2,player1);
            	printf("\nA %s le quedan %g puntos de vida\n",player1,player1vida);
            	}
               else
               {
               golpeplayer2=((FUE2+arma2)*azar2)*critico2;
               if(golpeplayer2<0)
                  	golpeplayer2=0;
          		player1vida-=golpeplayer2;
          		printf("\n%s da un Critico de:%g a %s\n",player2,golpeplayer2,player1);
            	printf("\nA %s le quedan %g puntos de vida\n",player1,player1vida);
            	}
          	}
          	else
          		printf("\n%s intenta dar a %s pero ha eludido el golpe\n",player2,player1);
         }
      //Para Cura + cualquier golpe
      if(tipogolpe1==1&&tipogolpe2==2||tipogolpe1==3&&tipogolpe2==2||tipogolpe1==4&&tipogolpe2==2)
         {
         if(elusion1==0)
          	{

               if(GCritico1==0)
               	{
                  golpeplayer1=((FUE1+arma1)*azar1);
                  if(golpeplayer1<0)
                  	golpeplayer1=0;
          			player2vida-=golpeplayer1;
          			printf("\n%s da un golpe de:%g a %s\n",player1,golpeplayer1,player2);
            		printf("\nA %s le quedan %g puntos de vida\n",player2,player2vida);
                  }
               else
               	{
                  golpeplayer1=((FUE1+arma1)*azar1)*critico1;
                  if(golpeplayer1<0)
                  	golpeplayer1=0;
          			player2vida-=golpeplayer1;
                  printf("\n%s da un Critico de:%g a %s\n",player1,golpeplayer1,player2);
            		printf("\nA %s le quedan %g puntos de vida\n",player2,player2vida);
                  }
          	}
          	else
          		printf("\n%s intenta dar a %s pero ha eludido el golpe\n",player1,player2);

         player2vida=player2vida+puntosdecura2*critico2;
         printf("%s se cura %g puntos de vida\n",player2,puntosdecura2*critico2);
         printf("\nA %s le quedan %g puntos de vida\n",player2,player2vida);

         }


   if(tipogolpe1==3||tipogolpe1==4)//Vuelta a valores normales
   	FUE1+=2;
   if(tipogolpe2==3||tipogolpe2==4)//Vuelta a valores normales
   	FUE2+=2;



   }//Fin de cuenteo de rondas


}
}


void espacios (int n)
{
	printf("\n");
	for (int i=0;i<n;i++)
	{
   printf(" ");
	}
}
