using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Lampada_Teste
{
    class Lampada
    {
        public int Tensao;
        public string Tipo;
        private string Cor;
        private double Preço;
        public bool Acesa = false;

        public bool Ligar()
        {
            Acesa = true;
            return Acesa;
        }
        public bool Desligar()
        {
            Acesa = false;
            return Acesa;
        }

        static void Main(string[] args)

        {
            Lampada l1 = new Lampada();
            Lampada LampJoao = new Lampada();
            l1.Tensao = 100; l1.Tipo = "led";
            if (l1.Acesa == true)
            {
                Console.WriteLine("Acesa");
            }
            else
            {
                Console.WriteLine("Apagada");
            }    
        }
    }
}
