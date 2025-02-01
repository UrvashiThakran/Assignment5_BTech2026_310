# Assignment5_BTech2026_310

# Coding Questions : 01.01.25

OOPS:

Problem Statement:

Ques1:Employee Information

Platform Used:
Programiz

Approach:Encapsulation

Code1:
#include<bits/stdc++.h>
using namespace std;
class Employee
{
  private:
  string name;
  int Emp_ID;
  double salary;
  public:
  Employee(string s,int id,int sal)
  {
      name=s;
      id=Emp_ID;
      salary=sal;
  }
  void getName(string s)
  {
      name=s;
  }
  void getEmp_ID(int id)
  {
      Emp_ID=id;
  }
  void getSalary(int sal)
  {
      salary=sal;
  }
  string setName()
  {
      return name;
  }
  int setEmp_ID()
  {
      return Emp_ID;
  }
  int setSalary()
  {
      return salary;
  }
  void calculateSalary(double performanceRating)
  {
      if(performanceRating>=0.0 && performanceRating<=1.4)
      {
          salary*=performanceRating;//calculate updated salary
      }
      else
      {
          cout<<"Invalid performance rating .Salary remains unchanged"<<endl;
      }
  }
};
int main()
{
    Employee e("RadhaRaman",12345,120000);
    e.getName("KunjBihari");
    cout<<"Name :"<<e.setName()<<endl;
    e.getEmp_ID(123456);
    cout<<"Employee ID:"<<e.setEmp_ID()<<endl;
    e.getSalary(12000);
    cout<<"Initial Salary :"<<e.setSalary()<<endl;
    e.calculateSalary(0.5);
    cout<<"Updated Salary :"<<e.setSalary()<<endl;
    return  0;
}

DBMS:

Platform Used:LeetCode

 Ques 1:Sales Person

 Code 1:

SELECT name 
FROM SalesPerson
WHERE sales_id NOT IN (
    SELECT sales_id 
    FROM Orders o 
    JOIN Company c ON o.com_id = c.com_id AND c.name = "RED");


 DSA:

 
