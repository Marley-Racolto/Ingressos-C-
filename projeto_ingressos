class program
{
    class Ingresso
    {
        public float Reais = 32f;
        public void ImprimiValor()
        {
            Console.WriteLine(Reais);

        }
        public class VIP : Ingresso
        {
            public float valorAdicional { get; set; }
            public float ImprimiValorAdc()
            {
                valorAdicional = 100f;
                return Reais + valorAdicional;
            }
        }
        public class Normal : Ingresso
        {
            public float ingressoNormal { get; set; }
            public float IngressoNormal()
            {
                ingressoNormal = Reais;
                return Reais;
            }
        }
        public class CamaroteInferior : VIP
        {
            public string LocalizacaoIngresso = "Setor 12 Seção 4";
            public float ValorADD { get; set; }
            public float ValorCamaroteInf()
            {
                float ValorADD = 55f;

                return (ValorADD + Reais);

            }
        }
        public class CamaroteSuperior : VIP
        {
            public float ValorAdc { get; set; }
            public float RetornarValor()
            {
                ValorAdc = 45f;
                return Reais + ValorAdc;

            }
        }
        static void Main(string[] Args)
        {
            int opcao;

            Normal ticket = new Normal();
            VIP vip = new VIP();
            CamaroteSuperior camaroteSUP = new CamaroteSuperior();
            CamaroteInferior camaroteINF = new CamaroteInferior();



            do
            {
                Console.Clear();

                ticket.ingressoNormal = ticket.IngressoNormal();
                Console.WriteLine($"Ingresso Normal: {ticket.IngressoNormal():F2}");

                vip.valorAdicional = vip.ImprimiValorAdc();
                Console.WriteLine($"Ingresso VIP: {vip.ImprimiValorAdc():F2}");

                camaroteSUP.ValorAdc = camaroteSUP.RetornarValor();
                Console.WriteLine($"Ingresso Camarote Superior: {camaroteSUP.ValorAdc:F2}");

                camaroteINF.ValorADD = camaroteINF.ValorCamaroteInf();
                Console.WriteLine($"Ingresso Camarote Inferior: {camaroteINF.ValorCamaroteInf():F2}");

                Console.WriteLine("");

                Console.WriteLine("1 - Normal");
                Console.WriteLine("2 - VIP");
                Console.WriteLine("3 - Camarote Superior");
                Console.WriteLine("4 - Camarote Inferior");
                Console.WriteLine("5 - Sair");

                opcao = int.Parse(Console.ReadLine());

                switch (opcao)
                {

                    case 1:

                        ticket.ingressoNormal = ticket.IngressoNormal();
                        Console.WriteLine($"Parabéns, você comprou o ingresso normal R$ {ticket.IngressoNormal():F2}");
                        Console.ReadKey();
                        break;


                    case 2:

                        vip.valorAdicional = vip.ImprimiValorAdc();
                        Console.WriteLine($"Parabéns, você comprou o ingresso VIP R$ {vip.ImprimiValorAdc():F2}");
                        Console.ReadKey();
                        break;


                    case 3:


                        camaroteSUP.ValorAdc = camaroteSUP.RetornarValor();
                        Console.WriteLine($"Parabéns, você comprou o ingresso Camarote Superior R$ {camaroteSUP.ValorAdc:F2}");
                        Console.ReadKey();
                        break;


                    case 4:

                        camaroteINF.ValorADD = camaroteINF.ValorCamaroteInf();
                        Console.WriteLine($"Parabéns, você comprou o ingresso Camarote Inferior R$ {camaroteINF.ValorCamaroteInf():F2}");
                        Console.WriteLine("Com localizaçao: {0}", camaroteINF.LocalizacaoIngresso);
                        Console.ReadKey();
                        break;



                }



            } while (opcao != 5);


        }
    }
}
