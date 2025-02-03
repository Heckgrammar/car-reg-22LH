 int charge = 0;
        Console.Write("Enter your car registration: ");
        string carReg = Console.ReadLine();
        while (carReg.Length > 8)
        {
            string displayMessage = carReg + " is not valid"; 
            Console.WriteLine(displayMessage);
            Console.Write("Enter a valid car registration: ");
            carReg = Console.ReadLine();
        }
        Console.Write("Enter your stay in hours: ");
        int hours = Convert.ToInt32(Console.ReadLine());
        if (hours < 2)
        {
            charge = 0;
        }
        else
        {
            charge = (hours * 2) + 2;
        }
        Console.WriteLine("parking charge: £" + charge);

![image](https://github.com/user-attachments/assets/f88e3166-4554-4a0b-85ac-ac155436f57e)
![image](https://github.com/user-attachments/assets/fcfc3db1-8849-4042-b772-cb864ae6c514)


