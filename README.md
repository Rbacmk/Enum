# Enum
 //Enum-Sıralama
            Console.WriteLine(Günler.Pazar);// Pazar gününü ekrana yazdırır.
            Console.WriteLine((int)Günler.Cumartesi);// Kaçıncı gün olduğunu yazar.
            int sıcaklık = 32;
            if (sıcaklık <= (int)HavaDurumu.Normal)
            {
                Console.WriteLine("Dışarı çıkmak için lütfen biraz daha havanın ısınmasını bekliyelim");
            }
            else if (sıcaklık >= (int)HavaDurumu.Sıcak)
            {
                Console.WriteLine("Dışarıya çıkmak için uygun hava ");
            }
            else if (sıcaklık >= (int)HavaDurumu.Normal && sıcaklık < (int)HavaDurumu.ÇokSıcak)
                Console.WriteLine("Hadi dışarı çıkalım!");

        }
    } enum Günler
    {
        Pazartesi,
        Salı,
        Çarşamba,
        Perşembe,
        Cuma,
        Cumartesi,
        Pazar
    }
    enum HavaDurumu
    {
        Soğuk=5,
        Normal=20,
        Sıcak=30,
        ÇokSıcak=40

    }
}
