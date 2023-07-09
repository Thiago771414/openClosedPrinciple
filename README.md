# Princípio Aberto-Fechado (Open-Closed Principle - OCP)

  O Princípio Aberto-Fechado (Open-Closed Principle - OCP) é um princípio de design de software que enfatiza a necessidade de as entidades do software serem abertas para extensão, mas fechadas para modificação. Isso significa que você deve ser capaz de adicionar novos recursos ou funcionalidades sem precisar modificar o código existente.

O OCP promove o uso de herança, interfaces e polimorfismo para alcançar essa extensibilidade. Em vez de modificar diretamente o código existente, você pode estender ou substituir partes específicas do sistema usando esses mecanismos.

Ao aplicar o OCP, você pode criar hierarquias de classes com uma classe base abstrata ou uma interface definindo o comportamento geral. Em seguida, você pode estender essa classe base ou implementar a interface para adicionar novas funcionalidades, mantendo a capacidade de interagir com o código existente sem modificá-lo.

Usando herança, você pode criar classes derivadas que adicionam comportamentos específicos ou substituem o comportamento padrão da classe base. Isso permite que você introduza novos recursos sem modificar o código existente, desde que a nova classe siga a mesma interface ou herança.

Interfaces são outro mecanismo essencial para o OCP. Ao definir interfaces claras e abstratas, você pode criar implementações diferentes para essas interfaces sem modificar o código existente que depende delas. Isso permite que você adicione novos comportamentos implementando a interface adequada, sem afetar o código existente.

O polimorfismo é uma consequência natural do uso de herança e interfaces. Ele permite que você trate objetos de diferentes classes de forma uniforme, usando a mesma interface comum. Dessa forma, você pode escrever código genérico que pode trabalhar com várias implementações diferentes, sem saber exatamente qual classe está sendo usada.

Em resumo, o Princípio Aberto-Fechado (OCP) promove a extensibilidade do software através do uso de herança, interfaces e polimorfismo. Ao adotar esse princípio, você pode adicionar novos recursos ou funcionalidades sem precisar modificar o código existente, o que torna o software mais flexível, modular e menos propenso a introduzir bugs ao modificar partes já funcionais do sistema.

```csharp
using System;

// Classe responsável por manipular dados de um estudante
public class Estudante
{
    public string Nome { get; set; }
    public int Idade { get; set; }
    public int Matricula { get; set; }
}

// Classe responsável por persistir os dados do estudante em um banco de dados
public class EstudanteRepository
{
    public void SalvarEstudante(Estudante estudante)
    {
        // Lógica para salvar o estudante no banco de dados
        Console.WriteLine("Estudante salvo no banco de dados.");
    }
}

// Classe responsável por exibir informações sobre o estudante
public class EstudanteInfoPrinter
{
    public void ImprimirInformacoes(Estudante estudante)
    {
        // Lógica para imprimir as informações do estudante
        Console.WriteLine($"Nome: {estudante.Nome}");
        Console.WriteLine($"Idade: {estudante.Idade}");
        Console.WriteLine($"Matrícula: {estudante.Matricula}");
    }
}

// Classe principal
public class Program
{
    public static void Main()
    {
        Estudante estudante = new Estudante
        {
            Nome = "João",
            Idade = 20,
            Matricula = 12345
        };

        EstudanteRepository repository = new EstudanteRepository();
        repository.SalvarEstudante(estudante);

        EstudanteInfoPrinter printer = new EstudanteInfoPrinter();
        printer.ImprimirInformacoes(estudante);
    }
}
```

## Livro
![Imagem](https://m.media-amazon.com/images/I/51YTqGVOD7L._SY425_.jpg)

# Autor
Thiago Reis Lima
https://www.linkedin.com/in/thiago-lima-2a5896166/
