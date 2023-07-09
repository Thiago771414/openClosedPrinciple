# Princípio Aberto-Fechado (Open-Closed Principle - OCP)

  O Princípio Aberto-Fechado (Open-Closed Principle - OCP) é um princípio de design de software que enfatiza a necessidade de as entidades do software serem abertas para extensão, mas fechadas para modificação. Isso significa que você deve ser capaz de adicionar novos recursos ou funcionalidades sem precisar modificar o código existente.

O OCP promove o uso de herança, interfaces e polimorfismo para alcançar essa extensibilidade. Em vez de modificar diretamente o código existente, você pode estender ou substituir partes específicas do sistema usando esses mecanismos.

Ao aplicar o OCP, você pode criar hierarquias de classes com uma classe base abstrata ou uma interface definindo o comportamento geral. Em seguida, você pode estender essa classe base ou implementar a interface para adicionar novas funcionalidades, mantendo a capacidade de interagir com o código existente sem modificá-lo.

Usando herança, você pode criar classes derivadas que adicionam comportamentos específicos ou substituem o comportamento padrão da classe base. Isso permite que você introduza novos recursos sem modificar o código existente, desde que a nova classe siga a mesma interface ou herança.

Interfaces são outro mecanismo essencial para o OCP. Ao definir interfaces claras e abstratas, você pode criar implementações diferentes para essas interfaces sem modificar o código existente que depende delas. Isso permite que você adicione novos comportamentos implementando a interface adequada, sem afetar o código existente.

O polimorfismo é uma consequência natural do uso de herança e interfaces. Ele permite que você trate objetos de diferentes classes de forma uniforme, usando a mesma interface comum. Dessa forma, você pode escrever código genérico que pode trabalhar com várias implementações diferentes, sem saber exatamente qual classe está sendo usada.

Em resumo, o Princípio Aberto-Fechado (OCP) promove a extensibilidade do software através do uso de herança, interfaces e polimorfismo. Ao adotar esse princípio, você pode adicionar novos recursos ou funcionalidades sem precisar modificar o código existente, o que torna o software mais flexível, modular e menos propenso a introduzir bugs ao modificar partes já funcionais do sistema.

## Livro
![Imagem](https://m.media-amazon.com/images/I/51YTqGVOD7L._SY425_.jpg)

# Autor
Thiago Reis Lima
https://www.linkedin.com/in/thiago-lima-2a5896166/
