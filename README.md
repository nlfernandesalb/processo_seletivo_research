# processo_seletivo_research
Desafio/ teste para estágio 

### Informações sobre a Automação para Criação de Relatório PDF por meio de um documento Word

#### Propósito

O objetivo principal deste código é automatizar a criação de um relatório em PDF que lista os fundos de investimento pertencentes à Família Trend (no caso em específico). Este relatório inclui as seguintes informações para cada fundo:

1. **Sugestão do fundo para cada classe de ativo.**
2. **Motivo pelo qual o fundo foi indicado.**
3. **Um disclaimer sobre o fundo.**

A automação foi concebida para ser utilizada por pessoas com conhecimentos básicos de programação, sendo o código amplamente documentado e comentado para facilitar o uso e a compreensão.

#### Funcionalidades do Código

1. **Leitura de Documento Word**:
   - O código começa lendo um arquivo no formato Word que contém a lista de fundos e suas explicações. A leitura é realizada utilizando a biblioteca `python-docx`, que permite extrair o conteúdo dos parágrafos do documento.

2. **Processamento dos Dados**:
   - O conteúdo extraído do documento é processado e organizado, categorizando os fundos de investimento, suas descrições e disclaimers. O código identifica as diferentes seções do documento e as organiza de modo que possam ser inseridas de forma estruturada no relatório PDF.

3. **Criação do Relatório em PDF**:
   - Após o processamento do conteúdo, o código gera um relatório em PDF. A capa do relatório é criada automaticamente, incluindo título, data e logotipo da empresa. Em seguida, o conteúdo é adicionado ao PDF, apresentando os fundos, suas descrições e disclaimers de maneira clara e organizada.
   - A biblioteca `FPDF` é utilizada para criar o PDF, permitindo a personalização de margens, fontes, cores e layout.

#### Como Utilizar o Código

1. **Configuração do Ambiente**:
   - Certifique-se de que as bibliotecas necessárias estão instaladas. As bibliotecas essenciais são `python-docx`, `FPDF`, e `reportlab`, que podem ser instaladas com o comando `pip install`.
   - Certifique-se também que o link clicável disposto como "Confira nossa visão para essa classe de ativo aqui" esteja atualizado.
   - Por utimo,os documentos '.docx' e a imagem da logo tem que estar disponíveis nos arquivos do ambiente de execução para que o código rode sem interrupções.

2. **Execução da Automação**:
   - O código pode ser executado em diversas plataformas Python, como:

     - **Jupyter Notebook**: As células podem ser executadas em sequência, começando com a importação das bibliotecas até a geração do PDF.
     - **Google Colab**: O código pode ser copiado para um notebook no Google Colab e executado da mesma forma. O Colab oferece a vantagem de um ambiente Python já configurado e permite o upload direto do arquivo Word.
     - **Script Python (.py)**: O código pode ser salvo em um arquivo `.py` e executado no terminal ou prompt de comando usando `python nome_do_arquivo.py`. O arquivo Word deve estar na mesma pasta que o script, ou o caminho correto deve ser fornecido.

  O único requisito é fornecer o arquivo Word com a lista de fundos e descrições. A estrutura do documento deve ser mantida para que o código funcione corretamente, mesmo que o conteúdo seja atualizado mensalmente.

3. **Geração do Relatório**:
   - Após a execução, um arquivo PDF será gerado automaticamente com o nome especificado (`Relatorio_Investimentos.pdf`). O relatório incluirá todas as informações organizadas de acordo com os requisitos definidos.

#### Como o Código Atende aos Requisitos

1. **Facilidade de Uso**:
   - O código está documentado com explicações em negrito, tornando-o acessível para pessoas com pouca experiência em programação. Isso garante que qualquer pessoa consiga entender e executar a automação com facilidade.
  
2. **Documentação Clara**:
   - O código é organizado e bem documentado, com explicações de cada função e seu papel na geração do relatório final.
  
3. **Execução Simples**:
   - O processo foi simplificado para exigir apenas a execução do código com o arquivo Word de entrada. Não é necessário modificar o código a cada mês, a menos que ocorram mudanças significativas na estrutura do documento, o que foi considerado no design da automação.

#### Considerações Finais

Este código oferece uma solução eficaz e acessível para a criação automatizada de relatórios de investimentos em PDF. Ele foi projetado para ser fácil de usar, permitindo que pessoas com pouca experiência em programação possam utilizá-lo sem dificuldades. Com a execução periódica, o relatório pode ser atualizado conforme necessário, mantendo a consistência e a qualidade das informações.
