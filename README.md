# Konspekt_Danila.Kotsalainen_ITKpv25_2
Konspekt

using System.ComponentModel.Design;

namespace MinuKonspekt
{
    internal class Program
    {
        static void Main(string[] args)
        {
            //Console.WriteLine("Hello, World!");

            //Muutujad, Matemaatilised tehted, IF, ELSE IF JA ELSE: 
           
            //1. tuvasta sisu võrdluses tühja stringiga, string andmetüüp
            Console.WriteLine("Tere kasutaja, mis on sinu nimi");
            string nimi = Console.ReadLine();

            if (nimi != null)
            {
                Console.WriteLine("Tere " + nimi + "!");

            }
            else if (nimi == "")
            {
                Console.WriteLine("Kasutaja ei sisestanud oma nime");
            }
            else
            {
                Console.WriteLine("Kasutaja ei sisestanud oma nime");
            }

            //2. tuvasta arvuvahemik, võrdluses piirvääartustega, int/double/float andmetüüp
            Console.WriteLine(nimi + ", mis on sinu vanus?");
            int kasutajavanus = int.Parse(Console.ReadLine());
            
            //2.1 mitu tingimust pesastatud if-ide abil
            //if (kasutajavanus > 0)
            //{
            //    if  (kasutajajavanus < 18)
            //    {
            //         Console.WriteLine("kashjuks energiajooki sulle ei müüda, oled Monsterist ilma 😐");
            //    }
            //    else
            //    {
            //         Console.WriteLine("Saad osta Monsterit, YIPPIE ");
            //    }
            //)
            //2.2 mitu tingimust ühe ifi sees kasudes loogilist tehet "and", vältides pesastamist
            if (kasutajavanus > 0 && kasutajavanus < 18)
            {
                  Console.WriteLine("kashjuks energiajooki sulle ei müüda, oled Monsterist ilma 😐");
            }
            else
            {
                  Console.WriteLine("Saad osta Monsterit, YIPPIE");
            }
            Console.WriteLine("Sisesta oma pikkus ka, palun, " + nimi + "");
            double pikkus = double.Parse(Console.ReadLine());
            if (pikkus < 1.00d)
            {
                Console.WriteLine("Oled juntsu");
            }
            else if (pikkus <1.25d && pikkus > 1.00d)
            {
                Console.WriteLine("Oled peaaegu allameetrimees");
            }
            else if (pikkus <1.50d && pikkus >1.25d)
            {
                Console.WriteLine("Oioi, päkapikk enam ei olegi " + nimi + " !");
            }
            else if (pikkus <1.75d && pikkus >1.75d)
            {
                Console.WriteLine("Pikk kolge, vaata et sa pead vastu uksepiita ära ei löö.");
            }
            else if (pikkus > 2.00d)
            {
                Console.WriteLine("Täielik tulnukas, kuidas pilved välja näevad?");
            }
            else
            {
                Console.WriteLine("pikkust ei tunta");
            }

        }
    }
}

