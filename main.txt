using System;
using System.Collections.Generic;
namespace dictionary
{
    class Program
    {
        static void Main(string[] args)
        {
            //System.Collections.Generic
            //Values lar uniq olmalı
            // keys ve values değerleri vardır

            Dictionary<int ,string> kullanıcılar = new Dictionary<int, string>();

            kullanıcılar.Add(10,"Ayşe Yılmaz");
            kullanıcılar.Add(12,"Ahmet Yılmaz");
            kullanıcılar.Add(18, "Deniz Arda");
            kullanıcılar.Add(20,"Özcan Coşar");

            //Dizinin Elemanlarına Erişim
            Console.WriteLine("********elemanlara erişim****");
            Console.WriteLine(kullanıcılar[18]);
            foreach (var item in kullanıcılar)
            {
                Console.WriteLine(item);
            }

            //Count
            Console.WriteLine("*******count*******");
            Console.WriteLine(kullanıcılar.Count);

            //Contains
            Console.WriteLine("*******contains*******");
            Console.WriteLine(kullanıcılar.ContainsKey(12));
            Console.WriteLine(kullanıcılar.ContainsValue("Cansel Gürsoy"));

            //Remove
            Console.WriteLine("*********remove********");
            kullanıcılar.Remove(12);
            foreach (var item in kullanıcılar)
            {
                Console.WriteLine(item);
            }

            //Keys
            Console.WriteLine("*********keys********");
            foreach (var item in kullanıcılar.Keys)
            {
                Console.WriteLine(item);
            }

            //Values
            Console.WriteLine("********values*****");
            foreach (var item in kullanıcılar.Values)
            {
                Console.WriteLine(item);
            }







        }
    }
}
