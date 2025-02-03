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
