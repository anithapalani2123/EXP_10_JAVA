
## EXP-10 -> DATA MEMBERS IN CLASS
## AIM:
To Write a Java program to create a class.
```
Create a class named 'Member' having the following members:
Data members:
1 - Name
2 - Age
3 - Phone number
4 - Address
5 - Salary

It also has a method named 'printSalary' which prints the salary of the members.
Two classes 'Employee' and 'Manager' inherits the 'Member' class. The 'Employee' and 
'Manager' classes have data members 'specialization' and 'department' respectively. 
Now, assign name, age, phone number, address and salary to an employee and
a manager by making an object of both of these classes and print the same.
```

## SOFTWARE REQUIRED :
IntelliJ IDEA COMMUNITY EDITION

## ALGORITHM:
```
Create a class named 'Member'.
Add the following data members to the 'Member' class: Name (String), Age (int), Phone number (String), Address (String), Salary (double).
Add a method named 'printSalary' to the 'Member' class, Inside the method, print the value of the 'Salary' data member.
Create a class named 'Employee' that inherits from the 'Member' class.
Create a class named 'Manager' that also inherits from the 'Member' class.
In the 'Main' class, create an object of the 'Employee' class and name it 'employee'. Assign values to the data members of 'employee'. Create an object of the 'Manager' class and name it 'manager'.Assign values to the data members of 'manager'
Call the 'printSalary' method for both 'employee' and 'manager' objects to print their salaries.
```



## PROGRAM:
### MEMBER.JAVA
```
public class Member
{
    public void Name(String name)
    {
        System.out.println(name);
    }
    public void Age(int age)
    {
        System.out.println(age);
    }
    public void PhoneNumber(String num)
    {
        System.out.println(num);
    }
    public void Address(String adrs)
    {
        System.out.println(adrs);
    }
    public void printSalary(int salary)
    {
        System.out.println(salary);
    }
}
```
### EMPLOYEE.JAVA
```
public class Employee extends Member
{
    public void specialization(String specialization)
    {
        System.out.println(specialization);
    }
}
```
### MANAGER.JAVA
```
public class Manager extends Member
{
    public void Department(String dept)
    {
        System.out.println(dept);
    }
}
```
### DETAILS.JAVA

```
public class Details
{
    public static void main(String[] args)
    {
        System.out.println("Employee Details: ");
        Employee emp = new Employee();
        emp.Name("Kaz");
        emp.Age(21);
        emp.PhoneNumber("9873321560");
        emp.Address("Pune");
        emp.printSalary(27000);
        emp.specialization("Software Designer");
        System.out.print("\n");
        System.out.println("Manager Details: ");
        Manager man = new Manager();
        man.Name("Inej");
        man.Age(23);
        man.PhoneNumber("7852291046");
        man.Address("Mumbai");
        man.printSalary(50000);
        man.Department("AI Developer");

    }
}
```



## OUTPUT:
![image](https://github.com/anithapalani2123/EXP_10_JAVA/assets/94184990/e54eb2fc-737f-40e3-8306-26e1768abf5e)


## RESULT:
Thus, the output is verified.
















