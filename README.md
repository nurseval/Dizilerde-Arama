# Dizilerde-Arama
Dizi içerisinde verilen elemanları bulma
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;





    namespace dizilerdearama


    internal class Program


    {
        static void Main(string[] args)

        {
            int i, id = -1; 

            /*-1 i atamadığım zaman id nin alacağı değer belli değil. yani şarta göre atama yapıyorum şart sağlanmazsa ne yapacağını söylemiyorum. */

            string ad;

            string[] isimler = { "Nur", "Dilek", "Ayhan", "Sibel", "Ayşegül", "Gül", "Hilal", "Bahar", "Vural", "Ahmet" }; 
            
            /*veriler string olduğu için her veri çift tırnak içinde olmalı */

            string[] tckn = { "100", "200", "300", "400", "500", "600", "700", "800", "900", "010" };

            Console.Write("Aradığınız İsim : ");

            ad = Console.ReadLine();

            for(i= 0; i< isimler.Length; i++)
            {
                if(ad==isimler[i])
                {
                    id = i;
                }
            }
            if (id >= 0)
            {
                Console.WriteLine("KİŞİNİN TC numarası :" + tckn[id]);
                Console.WriteLine("Kişinin Kayıt Numarası : " + id);
            }
            else
            {
                Console.WriteLine("Aradığınız Kişi Listede Bulunamamıştır.!");
            }
            Console.ReadKey();

                
        }
    }



[Patika Dev Sayfam](https://app.patika.dev/sevaalnuur)