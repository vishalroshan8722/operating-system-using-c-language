# operating-system-using-c-language                                                                                            
This c# source code will execute the demo of os that is loading processes, spy user friend, simple apps like calulator,creating the files, reading the file and modifing the file and tells system timing in each processs                                     
#include<math.h>
#include<time>
#include<dos.h>
void user();void files();void imfor();void dest2();
void calu();void spy();void please();void file();
void dest1();void spy1();void calim();void fileim();
void calim()
{int start1;
printf("-------------------------------------------------------------------------------\n");
printf("|     IMFORMATION                                 |\n");
printf("-------------------------------------------------------------------------------\n");
printf("points to operate the the calulator\n");
printf("->ONLY TWO OPERANDS CAN PERFORMED\n->THERE ARE FOUR OPERATIONS CAN PERFORMED\n* PRESS 1 TO ADDITION\n* PRESS 2 TO SUDRACTION\n* PRESS 3 TO MULTIPICATION\n* PRESS 4 TO DIVISION\n");
printf("ENTER 1 TO START \n>>>");scanf("%d",&start1);
}
void fileim()
{int start2;printf("-------------------------------------------------------------------------------\n");
printf("|     IMFORMATION                                 |\n");
printf("-------------------------------------------------------------------------------\n");
printf("points to operate the the file.txt files");
printf("->PRESS 1 TO WRITE(to type the contents in that file)\n * AFTHER FINISHING TYPEING THE IMFORMATION TO SAVE AND EXIST FORM THE FILE THEN PRESS THE CTRL+Z AND PREE ENTER KEY\n->PRESS 2 TO READ(it will displays the contents in thst file)\n");
printf("ENTER 1 TO START \n>>>");scanf("%d",&start2);
}
void imfor(){
clrscr();int start;printf("-------------------------------------------------------------------------------\n");
printf("|          IMFORMATION                            |\n");
printf("-------------------------------------------------------------------------------\n");
printf("READ THE FOLLOWING INSTRUCTION BEFORE GOING OS\n");
printf("->whenever '>>' this symdol dislpays the above methods should be follow\n”);
printf("->Select proper user account  for proper user name and respective password to avoid ");
printf("NOTE*USNAME1=user1*USNAME2=user2\n*PASSWD1=123*PASSWD2=1234\n");
printf("  Press (1 or 0) to start the operating system\n>>>");scanf("%d",&start);
}

void dest2(){int sel2,app2,drive1,power2;clrscr();please();clrscr();
 printf("--------------------------------------------------------------------------------");
 printf("\n\n1.APPLICATIONS\t\t2.MYCOMPUTER\t\t3.POWER OFF\n>>>"); scanf("%d",&sel2);
 if(sel2==1){clrscr();
 printf("-------------------------------------------------------------------------------");
 printf("\n\t\t  PATH:/USER ACCOUNT1/DESTOP/APPLICATION\n");
 printf("-----------------------------------------------------------------------------\n");
 printf("1.calucator\t2.fil1.txt\n>>>");scanf("%d",&app2);
 if(app2==1)
 {clrscr();calim();calu();
 }
 if(app2==2){clrscr();fileim();file();
 }}
 if(sel2==2)
 {clrscr();
 printf("-------------------------------------------------------------------------------");
 printf("\n\t\t\tPATH:/USER ACCOUNT1/DESTOP/MY COMPUTER\n" );
 printf("-------------------------------------------------------------------------------\n");
 printf("C DRIVE- [0MB USED OUT OF 100GB]\n");
 printf("D DRIVE- [0MB USED OUT OF 100GB]\n");
 printf("E DRIVE- [0MB USED OUT OF 100GB]\n");
 printf("F DRIVE- [0MB USED OUT OF 100GB]\n");
 printf(">>");scanf("%d",&drive1);dest2();
}if(sel2==3)
 {clrscr();
   printf("-------------------------------------------------------------------------------");
   printf("\n\t\t\tPATH:/USER ACCOUNT1/DESTOP/POWER OFF\n" );
   printf("-------------------------------------------------------------------------------\n");
   printf("1.SHUTDOWN  2.LOG OUT\n>>>");scanf("%d",&power2);
   clrscr();
   if(power2==1){
   printf("-------------------------------------------------------------------------------");
   printf("\n\nPREPARING TO SHUTDOWNING");
printf(".");delay(1000);printf(".");delay(1000);printf(".");delay(1000);
printf(".");delay(1000);printf(".");delay(1000);exit(0);
 }}getch();
}

void dest1(){}

void file(){FILE *file;char temp;int choice,num2=1;clrscr();
while(num2){clrscr();
printf("-------------------------------------------------------------------------------");
printf("\n\t\t\tPATH:/USER ACCOUNT1/DESTOP/POWER OFF/FILE1.TXT\n" );
printf("-------------------------------------------------------------------------------\n");
printf("Enter 1: Write \nEnter 2: Read\nEnter Your choice: ");scanf("%d", &choice);
switch(choice) {case 1:file = fopen("FiletestRecord.txt", "w");
if (file == NULL) {
	printf("\nFile can not be created");
} else {printf("\nPlease enter file content \n");
	while(scanf("%c", &temp) != EOF) {
		fprintf(file, "%c", temp); }
	printf("\n ----------------");
}
fclose(file);
	break;
case 2:printf("\n--------------- YOUR FILE CONTENT -------------------\n");
	file = fopen("FiletestRecord.txt", "r");
	if (file == NULL) {
		printf("\nCould not find file.");
	} else {int c;
		while((c = fgetc(file)) != EOF) {	printf("%c", c);
		}
	printf("\n-------------------FILE OVER-------------------------\n");
	}break;
}Printf(">>");scanf("%d",&num2);
}getch();dest1();
}

void files(){}

void user()
{clrscr();
printf("...............................................................................");
printf(":: ***USER_ACCOUNT_IS_SELECTED*** ::\n");
printf("...............................................................................");
}

void calu()
{   int oper,num=1;double firstNumber,secondNumber;
    clrscr();
    printf("-------------------------------------------------------------------------------");
    printf("\n\t\t\t\tPATH:/USER ACCOUNT1/DESTOP/APPLICATIONS\n" );
    printf("-------------------------------------------------------------------------------\n");
    while(num){printf("operations to perform \n PRESS 1. +(ADDITION):\n PRESS 2. -(SUBRACTION):\n PRESS 3. *(MULTIPILCATION):\n PRESS 4. /(DIVISION):\n>>>");
    scanf("%d",&oper);
    printf("Enter two operand 1: ");scanf("%lf",&firstNumber);
    printf("Enter two operand 2: ");scanf("%lf",&secondNumber);
    switch(oper){case1:printf("%.1lf+%.1lf=%.1lf\n",firstNu,secondNu, firstNu + secondNu;
	    break;
	case 2: printf("%.1lf+%.1lf=%.1lf\n",firstNu,secondNu, firstNu -secondNu;
	    break;
	case 3:printf("%.1lf*%.1lf =%.1lf\n",firstNu, secondNu, firstNu * secondNu);
	    break;
	case4:printf("%.1lf/%.1lf=%.1lf\n",firstNu, secondNu, firstNu / secondNu);
	    break;
	default:printf("Error! operator is not correct\n");
    } printf(">>");scanf("%d",&num);
    }getch();dest1();
    }
void please()
{printf("-------------------------------------------------------------------------------");
printf("\n\n\n\n\n\t\t\tPLEASE WAIT FOR MOMENT\t\t\t\t\n");
printf("\t\t\t\t.");delay(1000);printf(".");delay(1000)printf(".");delay(1000);
}
void spy(){
int des,tim,go;char name[10];
printf("-------------------------------------------------------------------------------");
printf("\n\n\n\n\n\t\t\tUSER LOG IN SUCESSFULL\n");delay(2000);clrscr();
printf("-------------------------------------------------------------------------------");
printf("\n\n\n\n\n\t\t                      WELCOME              ");
delay(1000);clrscr();please();
printf("--------------------------------------------------------------------------------");
for( int i=0;i<=10;i++){
i=i+5;printf("%d >> loaded >> 100%\n",i);delay(500);
}
printf("                    |      LOADING     |                 ");
printf("HI HIS IS *SPY,YOURSYSTEM LOADING[ 5%> outof >100%]     ");
printf("I HELP YOU TILL LOADED            | [10%> outof >100%]	  ");
printf("LET ME KNOW ABOUT YOUR NAME   [10%> outof >100%]    ");
printf(">>>");scanf("%s",name);
printf("%s YOUR PREVIOUS ACTIVITIES IN DESKTOP  ARE\n",name);
printf("file2.txt\ncalulator\nmy computer\n");
printf("....                                   | [40%> outof >100%]	        	");
delay(1000);printf(".");delay(1000);printf(".");delay(1000);
printf("YOUr PERSONAL THINGSLOADEDSUCCESSFULLY                                        ");
printf("YOU WANT TO GO TO DESKTOP [1.yes /2. no]                                        ");
printf(">>>");scanf("%d",&des);
switch (des){
case 1:clrscr();please();clrscr();
printf("--------------------------------------------------------------------------------");
printf("\n\n              WELCOME TO THE DESKTOP                            \n");
delay(2000);dest1();
break;
  case 2:delay(500);clrscr();
  printf("--------------------------------------------------------------------------------");
  printf("HI%s,ITS*SPYAGAINBACK",name);
  printf("%s U KNOW ABOUT WHAT TIME U STARTED\n [1-yes/2-no]\n",name);
  printf(">>>");scanf("%d",&tim);
  if (tim==1){
  time_t t;time(&t);
  printf("\n CURRENT TIME IS:%s:-",ctime(&t));
  printf("U STARTED 1min 22seconds BEFOR TO YOUR CURRENT TIMMING'S \n\n ");
  printf("->YOURSYSTEMISSUCCESFULLYLOADED->YOUWANTGOTOTHE DESKTOP\n");
  printf("+++++++PRESS 1 TO GO THE DESKTOP+++++++\n>>>");scanf("%d",&go);
  clrscr(); please();clrscr();
  printf("--------------------------------------------------------------------------------");
  printf("\n\WELCOMETOTHEDESKTOP” );delay(2000);dest1();
  }else{
   printf("YOU WANT TO GO TO DESKTOP");
   delay(2000); please();clrscr();
   printf("--------------------------------------------------------------------------------");
   printf("\n  WELCOME TO THE DESKTOP                            \n");
   delay(2000);dest1();
  }break;}}

 void spy1(){}

int main(){
int a,way, gm,count=1,times;char u1[10],p1[10],u2[10],p2[10];
clrscr();
printf("-------------------------------------------------------------------------------");
printf("\n\n\n\n\n\t\t\tPLEASE WAIT FOR THE MOMENT\t\t\t\t\n");printf("\t\t\t\t.");
delay(1000);printf(".");delay(1000);printf(".");delay(1000);printf(".");
delay(500);printf(".");delay(500);printf(".");delay(1000);printf(".");delay(1000);
clrscr();imfor();clrscr();please();clrscr();
while(count){
b:printf("--------------------------------------------------------------------------------");
printf("|\t\t\t**CHOOSE THE USER ACCOUNT**                           |\n");
printf("--------------------------------------------------------------------------------");
printf("\t\t1.USERNAME1           2.USERNAME2         3.EXIT\n");
printf( "\nSELECT THE USERNAME TO LOG IN:>>>" );a:scanf("%d",&a );
switch (a){
case 1:user();printf("");
printf("\n\t\t\t      USERNAME=");scanf("%s",u1);printf("");
printf("\n\t\t\t      PASSWORD=");scanf("%s",p1);
if(strcmp(u1,"user1")==0 && strcmp(p1,"123")==0)
{clrscr();spy();
}else{
printf("\nUSERNAME AND PASSWORD IS MISSMATCHED\n");
}break;
case 2:user();
printf("\n\t\t\t      USERNAME=");scanf("%s",u2);
printf("\n\t\t\t      PASSWORD=");scanf("%s",p2);
if(strcmp(u2,"user2")==0 && strcmp(p2,"1234")==0){
clrscr();spy1();
}else{printf("\nUSERNAME AND PASSWORD IS MISSMATCHED\n");
}break;
case 3:clrscr();
printf("\nCHOOSE THE WAY TO EXIT");
printf("\n1.SHUTDOWN          2.SLEEP\n");
printf("SELECT=");scanf("%d",&way);
delay(500);clrscr();
if(way==1){
printf("\n\nPREPARING TO SHUTDOWNING");
printf(".");delay(1000);printf(".");delay(1000);printf(".");
delay(1000);printf(".");
delay(1000);printf(".");
delay(1000);printf("  ");
delay(2000);exit(0);
}
if(way==2)
{
printf("NOTE:TIME_FORMAT_SHOULD_BE_IN_FORMAT:N000\n");
printf("FIX THE SLEEP TIME\n>>");
scanf("%d",&times);
clrscr();
delay(times);
goto b;
}
break;
default:
printf("\nINVALID!!!!!CHOICE ENTER CORRECT CHOICE\n>>>");
goto a;
}
printf(">>");
scanf("%d",&count);
clrscr();
}
getch();
}}
