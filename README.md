#include <stdio.h>
 
/*structure declaration*/
typedef struct
{
    char empname[30];
    char depname[30];
    int empno;
    float salary;
} Employee;
 
int main()
{
	  int n=20;int i;
    Employee emp[n];
    for(i=0; i<n; i++)
	 {
    printf("\nEnter details :\n");
    printf("Enter Name");          
	  gets(emp[i].empname);
    printf("Enter Employee ID");            
	  scanf("%d",&emp[i].empno);
    printf("Enter Salary");        
	  scanf("%f",&emp[i].salary);
	  printf("Enter Department");          
	  scanf("%s",&emp[i].depname);
	  char ch=getchar();
	  printf("\n");
   }
   
    printf("------EMPLOYEE DETAILS------");
    for(i=0; i<n; i++)
	  {
    printf("\n Name: %s",emp[i].empname);
    printf("\n ID: %d",emp[i].empno);
    printf("\n Salary: %f",emp[i].salary);
    printf("\n Department: %s \n",emp[i].depname);
    printf("\n -------------");
    printf("\n");
    }
    return 0;
}
