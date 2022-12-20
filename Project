#include <iostream>
#include <vector>
using namespace std;

vector<string>name;
vector<char>gender;
vector<int>age, salary;

void AddNewEmployee()
{
    string x;
    int n,s;
    char g;
    cout << "   enter the name of employee : ";
    cin >> x;
    name.push_back(x);
    cout << "   enter the age of employee : ";
    cin >> n;
    age.push_back(n);
    cout << "   enter the salary of employee : ";
    cin >> s;
    salary.push_back(s);
    cout << "   enter the gender of employee (f for female - m for male) : ";
    cin >> g;
    gender.push_back(g);
}


void PrintAllEmployes()
{
    
    if (name.empty()) cout << "   Data is empty" << endl;
    else {
        cout << "   ID                    Name                    Age                    Salary                    Gender" << endl;
        for (int i = 0;i < name.size();i++)
        {
            int x;
            cout << "   " << i + 1 << "                     ";
            cout << name[i];
            x = name[i].size();
            for (int i = 1;i <= 20 + 4 - x;i++)
            {
                cout << " ";
            }
            cout << age[i];
            for (int i = 1;i <= 21;i++)
            {
                cout << " ";
            }
            cout << salary[i];
            for (int i = 1;i <= 20 + 4;i++)
            {
                cout << " ";
            }
            cout << gender[i] << endl;
        }
    }
}

void DeleteByAge()
{
    int n;
    if (name.empty()) cout << "   Data is empty" << endl;
    else {
        cout << "   Enter the age you want to delete : ";
        cin >> n;
        for (int i = 0;i < name.size();i++)
        {
            if (age[i] == n)
            {
                name.erase(name.begin() + i);
                age.erase(age.begin() + i);
                salary.erase(salary.begin() + i);
                gender.erase(gender.begin() + i);
                i--;
            }
        }
    }
}

void UpdateSalaryByName()
{
    string x;
    int n;
    if (name.empty()) cout << "   Data is empty" << endl;
    else {
        cout << "   Enter the name you want to update salary : ";
        cin >> x;
        cout << "    Enter the new salary :  ";
        cin >> n;
        for (int i = 0;i < name.size();i++)
        {
            if (name[i] == x)
            {
                salary[i] = n;
            }
        }
    }
}


int main()
{

    int n;
    cout << "1) add new employee." << endl;
    cout << "2) print all employes." << endl;
    cout << "3) delete by age." << endl;
    cout << "4) update salary by name." << endl;
    cout << "Enter your choice (enter 0 if you need to exit) : ";
    cin >> n;
    while(n != 0)
    {
        if (n==1)
        {
            AddNewEmployee();
        }
        if (n == 2)
        {
            PrintAllEmployes();
        }
        if (n == 3)
        {
            DeleteByAge();
        }
        if (n == 4)
        {
            UpdateSalaryByName();
        }
        cout << "1) add new employee." << endl;
        cout << "2) print all employes." << endl;
        cout << "3) delete by age." << endl;
        cout << "4) update salary by name." << endl;
        cout << "Enter your choice (enter 0 if you need to exit) : ";
        cin >> n;
    }
    
}
