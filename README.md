# Notebook Didático de Tratamento de Exceções em Python 

Este repositório contém um guia didático e prático dedicado ao **tratamento de exceções e à construção de código robusto em Python**.  
O objetivo central do material é demonstrar como a gestão adequada de fluxos de erro contribui para o desenvolvimento de sistemas resilientes, capazes de lidar com estados inesperados sem interromper abruptamente a execução do programa.

## 📚 Fundamentação Teórica

O notebook aborda a distinção entre erros de escrita (*erros sintáticos*) e exceções ocorridas em tempo de execução, apresentando a taxonomia das principais classes de erro da linguagem Python:

- **SyntaxError**  
  - Erros de grafia ou estrutura no código
- **NameError**  
  - Tentativa de utilização de variáveis ou funções não definidas
- **IndexError**  
  - Acesso a índices fora do intervalo válido de uma lista
- **TypeError**  
  - Operações realizadas entre tipos de dados incompatíveis
- **KeyError**  
  - Tentativa de acesso a chaves inexistentes em dicionários
- **ValueError**  
  - Dados com tipo correto, mas que violam regras lógicas
- **ZeroDivisionError**  
  - Indeterminação matemática causada por divisão por zero

## 🏗️ Estrutura de Controle de Fluxo

O projeto demonstra a utilização da estrutura `try-except-else-finally`, analisando o ciclo de vida de uma exceção e seus impactos no fluxo do programa:

- **try**
  - Bloco de código suscetível à ocorrência de erros
- **except**
  - Fluxo de recuperação executado quando uma exceção é capturada
- **else**
  - Executado apenas quando o bloco `try` não gera exceções
- **finally**
  - Executado independentemente da ocorrência de erro, geralmente utilizado para liberação de recursos
- **raise**
  - Mecanismo para lançamento manual de exceções, permitindo validações personalizadas

## 🛠️ Aplicações Práticas e Estudos de Caso

Os conceitos teóricos são aplicados em cenários que simulam desafios reais da engenharia de software, tais como:

- **Busca de Estudantes**
  - Tratamento de `KeyError` em sistemas de consulta baseados em dicionários
- **Validação de Dados**
  - Uso de `raise ValueError` para impor restrições quantitativas em listas de notas
- **Processamento de Sinais**
  - Divisão de colunas de pressão e temperatura, com tratamento simultâneo de listas de tamanhos distintos e divisões por zero
- **Sanitização de Texto**
  - Identificação de caracteres e pontuações inválidas em strings por meio de exceções personalizadas
- **Conversão de Tipos**
  - Implementação de funções seguras para conversão de listas em valores `float`, com tratamento de erros de valor

## 🚀 Como utilizar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
2. Execute o notebook:
- Abra o arquivo python_excecao.ipynb no Google Colab ou Jupyter Notebook.
- Execute as células sequencialmente para acompanhar os exemplos e exercícios propostos.
