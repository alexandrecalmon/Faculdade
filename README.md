# Trabalho Acadêmico de Graduação Ciência de Dados

<html>
<head>
<title>Inserindo vídeos do YouTube em uma página HTML</title>
<meta http-equiv="Content-Type" content="text/html; charset=iso-8859-1">
</head>
<body>
<p>Meu vídeo preferido</p>
	<object style="height: 390px; width: 640px">
		<param name="movie" value="https://www.youtube.com/watch?v=xN9jOIfakVI&feature=youtu.be">
		<param name="allowFullScreen" value="true">
		<param name="allowScriptAccess" value="always">
		<embed src="https://www.youtube.com/watch?v=xN9jOIfakVI&feature=youtu.be" type="application/x-shockwave-flash" allowfullscreen="true" allowScriptAccess="always" width="640" height="360">
	</object>
	
	<object style="height: 390px; width: 640px">
</body>
</html>


### Repositórios dos exercícios do curso de Ciência de Dados

Esse notebook trabalha com os dados públicos da Mega-Sena, disponíveis no Portal de Loterias da Caixa Econômica Federal. Para baixar o arquivo atualizado basta clicar neste link.

Após baixar o arquivo, você precisa descompacta-lo para utilizar o arquivo <D_megase.html> neste notebook. Nesta análise não iremos incluir estudos sobre a Mega Sena da Virada.

Para a aquisição e análise dos dados, será utilizada a linguagem de programação Python e as bibliotecas Pandas, Numpy, Matplotlib, plotly.express e FuncFormatter.

Para executar esse notebook com todas as bibliotecas necessárias, basta baixar o Anaconda e utilizar a ferramenta Jupyter Notebook.

OBS: Se ao executar este notebook aparecer um erro Notebook validation: failed The save operation succeeded, but the notebook does not appear to be valid. The validation error was: bastar instalar esta atualização no prompt de comando do Anaconda pip install --upgrade nbformat ou executar no próprio Jupyter Notebook o comando !pip install --upgrade nbformat

### O que será analisado neste notebook

- As 5 maiores arrecadações da Mega Sena representado por um gráfico de barras.
- As 5 menores arrecadações da Mega Sena representado por um gráfico de barras.
- Os 5 maiores prêmios pagos pela Mega Sena representado por um gráfico de barras.
- Os 5 menores prêmios pagos pela Mega Sena representado por um gráfico de barras.
- Comparativo entre as variáveis arrecadação total, valores acumulados e prêmio total ao longo dos anos representado por um gráfico temporal. Iremos também informar abaixo do gráfico, em forma de percentual, qual o grau de correlação entre as variáveis.
- Comparativo entre as variáveis arrecadacao total, valor acumulado e prêmio total representado por um gráfico de dispersão.
- Quantidade de vezes em que cada dezena da Mega Sena foi sorteada representado por um gráfico de barras.
- Quantidade de ganhadores da Mega Sena dividido por estados representado por um gráfico treemap e um gráfico sunburst.
- Este conjunto de dados tem informações de todas as rodadas da loteria do Brasil que ocorreram desde 1996/03/11 (a primeira) até o número da loteria 2262 que ocorreu em 20/05/2020.

### O conteúdo desse conjunto de dados é basicamente:

- Id: identificação.
- Concurso: O número da loteria
- Data Sorteio: A data em que a rodada ocorreu
- 1ª Dezena: O primeiro número do sorteio
- 2ª Dezena: O segundo número do sorteio
- 3ª Dezena: O terceiro número do sorteio
- 4ª Dezena: O quarto número do sorteio
- 5ª Dezena: O número do quinto sorteio
- 6ª Dezena: O sexto número do sorteio
- Arrecadacao_Total: O total arrecadado de todos os apostadores para esta rodada da loteria
- Ganhadores_Sena: A quantidade de vencedores que atingiu pelo menos seis números nesta rodada
- Cidade: A cidade do vencedor
- UF: O estado do vencedor
- Rateio_Sena: O valor dividido para os vencedores
- Ganhadores_Quina: A quantidade de vencedores que atingiu cinco números
- Rateio_Quina: O valor dividido para os vencedores de cinco números
- Ganhadores_Quadra: A quantidade de vencedores que atingiu quatro números
- Rateio_Quadra: O valor dividido para os vencedores de quatro números
- Acumulado: Um campo "sim / não" que informa se essa rodada teve os valores acumulados para a próxima rodada
- Valor_Acumulado: o valor do dinheiro acumulado para a próxima rodada, se ninguém vencer esta rodada
- Estimativa_Prêmio: Uma estimativa do prêmio total
- Acumulado Mega da_Virada: Um valor acumulado que vale para uma modalidade especial da loteria
