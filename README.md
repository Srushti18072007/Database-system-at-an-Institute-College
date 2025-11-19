#include <stdio.h>

struct employee {
    char name[20];
    int id;
    char department[30];
    float salary;
};

int main() {
    struct employee e1, e2, e3, temp;

    printf("Enter details of Employee 1:\n");
    printf("Name: ");
    scanf("%s", e1.name);
    printf("ID: ");
    scanf("%d", &e1.id);
    printf("Department: ");
    scanf("%s", e1.department);
    printf("Salary: ");
    scanf("%f", &e1.salary);

    printf("\nEnter details of Employee 2:\n");
    printf("Name: ");
    scanf("%s", e2.name);
    printf("ID: ");
    scanf("%d", &e2.id);
    printf("Department: ");
    scanf("%s", e2.department);
    printf("Salary: ");
    scanf("%f", &e2.salary);

    printf("\nEnter details of Employee 3:\n");
    printf("Name: ");
    scanf("%s", e3.name);
    printf("ID: ");
    scanf("%d", &e3.id);
    printf("Department: ");
    scanf("%s", e3.department);
    printf("Salary: ");
    scanf("%f", &e3.salary);
 
 
    if (e1.salary > e2.salary)
    { temp = e1; e1 = e2; e2 = temp; }
    if (e2.salary > e3.salary)
    { temp = e2; e2 = e3; e3 = temp; }
    if (e1.salary > e2.salary)
    { temp = e1; e1 = e2; e2 = temp; }

    printf("\n\n========= SORTED BY SALARY IN ASCENDING ORDER =========\n");
    printf("\nEmployee 1: %s %d %s %f\n", e1.name, e1.id, e1.department, e1.salary);
    printf("Employee 2: %s %d %s %f\n", e2.name, e2.id, e2.department, e2.salary);
    printf("Employee 3: %s %d %s %f\n", e3.name, e3.id, e3.department, e3.salary);

    return 0;
}



