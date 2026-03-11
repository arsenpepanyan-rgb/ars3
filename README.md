# ars3
            Employee employee = new Employee("Arsen", "menejer", 100);
            employee.ChangeSalary(-50);
            employee.ShowInfo();
        }
    }
    class Employee
    {
        public string Name;
        public string JobTitle;
        public int Salary;

        public Employee(string name, string jobTitle, int salary)
        {
            Name = name;
            JobTitle = jobTitle;
            Salary = salary;
        }
        public void ChangeSalary(int changeSalary)
        {
            Salary = changeSalary;

            if(changeSalary < 0)
            {
                Console.WriteLine("Not valid salary");                
            }
        }

        public void ShowInfo()
        {
            Console.WriteLine($"Employee name: {Name}\nEmployee job title: {JobTitle}\nEmployee salary: {Salary}");
        }


    }

}
