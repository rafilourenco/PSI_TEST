# Teste de PSI Modelo

## Informação do aluno

    Nome: Rafael Lourenço

Teste termina às 09:40 (Turno 1) / 13:25 (Turno 2).

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### 1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    char c = '\u00AE';
    Console.WriteLine($@"\n{c}\n");

P1 - Resposta

    O código irá imprimir \n®\n o "®" que é unicode \u00AE é o simbolo da marca registada.Visto que tem o @ ou seja uma string verbatim e string literal, o \n não ira resultar, apenas aparece o simbolo \u00AE(®) pois existe uma interpolação com $ e está dentro de {}.


### 2. Considera o seguinte código

    double d = 0.3513;
    float f = 12.645;

    Console.WriteLine($"{d} + {f} = {d + f}");

### Indica a correção necessária para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

    Visto que a váriavel f é float, é necessario que o valor acabe com f, logo para que o código não apresente erros é necessário ser: float f = 12.645f; .

### 3. Escreve um programa que solicite uma string ao utilizador, e seguidamente a mostre no ecrã de forma invertida

P3 - Resposta

    string texto; // indicar a variavel

    Console.Write("Introduza um frase ou palavra: "); // Imprimir a solicitação da variavel.
    texto = Console.ReadLine(); // guardar a variavel introduzida pelo utilizador.

    for(int i = texto.Length - 1; i >= 0;i--){ // Ciclo For que percorre a string "texto" que é iterável, caracter a caracter usando "texto.Length", necessitando de percorrer ao contrário fazendo - 1 e de seguida i--; .
        Console.Write(texto[i]); // Imprimir o texto inverso.
    }


### 4. Quais são os comandos Git para configurares, de uma forma global, o teu **nome** e **email** para realização de *commits*? E se essa configuração for apenas para um repositório?

P4 - Resposta

    Para configurar de forma global o nome e o email é necessário utilizar os seguintes códigos: git config --global user.name "Nome" e git config --global user.email "Email".
    Para que seja apenas para um repositório é necessário substituir o "global" por nada, logo git config user.name "Nome" e git config user.email "Email".
