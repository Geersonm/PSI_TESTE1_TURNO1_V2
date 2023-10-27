# Teste de PSI 1 - Turno 1 - Versão 2

## Informação do aluno

    Nome: Gerson Monteiro

Teste termina às 10:45.

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### P1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    bool b = 5 < 2;
    double d = Convert.ToDouble(b);
    
    Console.WriteLine(d);

P1 - Resposta

    Sera impresso 0 isso ocorre porque o valor booleano da primeira linha é igual a false que foi convertido em um número double que representa 0.0.

### P2. Considera o seguinte código com um *bug*

    string s = "2.5";
    double d = Convert.ToInt32(s);

    Console.WriteLine(d);

### Indica uma possível correção para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

       A correção que devemos fazer é na linha 2 em vez de usar "Convert.ToInt32(s);" devemos usar "Convert.ToDouble(s);", porque ao fazer "Convert.ToInt32(s);" estamos adizer para converter 2,5 em um numero inteiro pois isso não é possivel porque é um numero real, então usamos "Convert.ToDouble(s);" que é o mais apropriado.
   
### P3. Escreve um programa que solicite ao utilizador dois números inteiros e os multiplique, apresentando o resultado. Caso este seja um número divisível por 3, deve também ser impressa a mensagem "Múltiplo de 3!"

P3 - Resposta

            int n1;
            int n2;
            int m;

           Console.WriteLine("Introduz um numero:");
           n1=int.Parse(Console.ReadLine());
           
           Console.WriteLine("\nIntroduza outro numero:");
           n2=int.Parse(Console.ReadLine());

           m=n1 * n2;

           Console.WriteLine($"\n{m}");

           if(m % 3 == 0)
           {
            Console.WriteLine("\nMúltiplo de 3!");
           }

### P4. Tens um repositório git criado localmente, onde estás no ramo 'master'. Queres associá-lo ao repositório remoto contido no url 'https://github.com/PSI/OMeuRepositorioRemotoV2'. Queres também alterar o nome do ramo atual para 'main'. Deverás enviar os *commits* já feitos localmente para o repositório remoto. Indica os comandos necessários

P4 - Resposta

    git remote add origin https://github.com/PSI/OMeuRepositorioRemotoV2
    git branch -M main
    git push -u origin main
