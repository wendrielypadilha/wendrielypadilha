using System;

class Program
{
    static void Main()
    {
        int a = 7;
        int b = a - 6;

        int[] v = new int[10]; // Ajuste o tamanho conforme necessário.

        while (b < a)
        {
            v[b] = b + a;
            b += 2; //  Incremente b em 2.
        }

        // Imprima os resultados opcionalmente.
        for (int i = 0; i < v.Length; i++)
        {
            if (v[i] != 0) // Imprima apenas os valores inicializados.
            {
                Console.WriteLine($"v[{i}] = {v[i]}");
            }
        }
    }
}
