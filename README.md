# ars3
        int number;
        int even;
        int odd;
        Console.Write("Viberite chislo Ot 0 do 100: ");
        number = Convert.ToInt32(Console.ReadLine());

        if(number > 100 || number < 0)
        {
            Console.WriteLine("Takova chisla netu");
            return;
        }
        if (number % 2 == 0)
        {
            even = number;
            Console.WriteLine("Eto chyotnoe chislo " + even);
        }
        else
        {
            odd = number;
            Console.WriteLine("Eto NE chyotnoye chislo " + odd);
        }

    }

}
