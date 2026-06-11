Assistente Inteligente para Triagem de Ocorrências Policiais

Objetivo:
Auxiliar a classificação inicial de ocorrências policiais por meio de Inteligência Artificial.

Limites:
- Não substitui o policial.
- Não toma decisões operacionais.
- Apenas sugere classificações.

Entradas:
- descrição

Saídas:
- natureza
- base legal
- ação recomendada

Workflow:

1. Receber descrição da ocorrência.
2. Identificar palavras-chave.
3. Classificar a natureza da ocorrência.
4. Consultar legislação relacionada.
5. Consultar procedimento recomendado.
6. Gerar resposta estruturada.

Critério de validação:

A classificação deve corresponder ao fato relatado e apresentar base legal e procedimento compatíveis.

Limites da IA:

- Não substitui o policial responsável.
- Não realiza prisões.
- Não toma decisões operacionais.
- Não acessa bancos de dados policiais.
- Não utiliza dados pessoais sensíveis.
- Apenas sugere classificações para apoio à triagem.

Privacidade e Segurança

O sistema não utiliza:

- Nome do solicitante
- CPF
- RG
- Endereço residencial
- Dados bancários
- Informações pessoais sensíveis

A análise é realizada apenas sobre a descrição da ocorrência.

Tool Calling

Ferramenta: consultar_legislacao

Objetivo:
Consultar a base legal relacionada à ocorrência identificada.

Exemplo:

Entrada:
{
  "tema": "violencia_domestica"
}

Saída:
{
  "artigo": "Art. 24-A da Lei Maria da Penha"
}

Ferramenta: consultar_procedimentos

Objetivo:
Consultar orientações operacionais iniciais.

Exemplo:

Entrada:
{
  "tema": "violencia_domestica"
}

Saída:
{
  "procedimento": "Deslocamento imediato da equipe"
}
