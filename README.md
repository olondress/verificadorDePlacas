# Verificador de Placas

Este projeto consiste em um sistema simples para verificação de placas de veículos, implementado em Java. Ele permite validar e formatar placas de acordo com os padrões estabelecidos, além de oferecer funcionalidades de busca e relatórios. O sistema utiliza arquivos .txt para persistência de dados e garantir que as verificações realizadas sejam armazenadas para futuras consultas.

## Índice
- [Descrição do Projeto](#descrição-do-projeto)
- [Funcionalidades](#funcionalidades)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Exemplo de Uso](#exemplo-de-uso)

## Descrição do Projeto
O objetivo principal deste projeto é fornecer uma interface para validar placas de veículos, garantindo conformidade com os padrões estabelecidos. O sistema permite verificar a autenticidade das placas, formatar corretamente os dados inseridos e gerar relatórios sobre as verificações realizadas.

## Funcionalidades
### Verificação de Placas
- **Validar placas**: Confere se a placa inserida está no formato correto.
- **Formatar placas**: Ajusta automaticamente o formato da placa, se necessário.
- **Buscar placas**: Permite buscar uma placa específica no histórico de verificações.
- **Gerar relatórios**: Cria um relatório detalhado com todas as placas verificadas.

### Persistência de Dados
O sistema utiliza a classe `ArquivoUtil` para leitura e gravação de arquivos .txt, garantindo que as verificações realizadas sejam salvas entre as sessões.

## Estrutura do Projeto
A estrutura de pastas e classes está organizada da seguinte forma:

```
src/
├── exceptions/
│   ├── PlacaInvalidaException.java
│
├── interfaces/
│   ├── Verificavel.java
│   ├── Formatavel.java
│   ├── Relatavel.java
│
├── models/
│   ├── Placa.java
│   ├── Verificacao.java
│
├── services/
│   ├── ArquivoUtil.java
│   ├── VerificadorPlacas.java
│
└── Main.java
```

## Tecnologias Utilizadas
- **Linguagem**: Java 8 ou superior
- **Persistência**: Arquivos .txt
- **Paradigma**: Programação Orientada a Objetos (POO)
- **Design**: Interface e abstração para modularidade

## Exemplo de Uso
Após executar o sistema, o usuário pode:
- Inserir uma placa para validação.
- Ver o resultado da validação e a formatação correta, caso necessário.
- Buscar no histórico se uma determinada placa já foi verificada.
- Gerar um relatório detalhado de todas as placas verificadas.
