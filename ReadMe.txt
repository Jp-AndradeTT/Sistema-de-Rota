Guia de Execução e Uso - Projeto de Inteligencia Artificial

		Sistema de Rota Inteligente


		
		Como rodar o projeto

1. Abra o projeto.

2. Após abrir o projeto no seu editor de código, é necessário estar baixando o requirements.txt, dando um pip install -r, assim baixando as bibliotecas necessárias.

3. O arquivo main esta a inicialização do servidor, com isso basta dar um python .\main.py que estará executando.
Logo após é necessário copiar o endereço e colar no seu navegador e assim estará executando o projeto.

Estrutura de Arquivos:

No diretório Templates está nosso index.html
No diretório static esta nosso script.js e nossa estilização do front, styles.css
O arquivo algoritmo.py responsável pela estrutura base e a lógica dos algoritmos de otimização
o arquivo ag_pcv.py está a estrutura do algoritmo genético
O arquivo main.py é o arquivo prinficpal da aplicação, contendo integração com a API Flask, mapeamento das rotas de comunicação com o front e inicialização do servidor. 





		Como utilizar a aplicação 

O sistema foi feito para ser interativo. Siga os passos abaixo para realizar suas simulações:

	1. Mapeamento dos Pontos (Cidades)

Primeiro, deve interagir com a interface para determinar os pontos.
Cada ponto inserido na tela representará uma "cidade" ou um nó no qual os algoritmos farão os cálculos de rota/otimização.

	2. Seleção e Configuração Individual

Após definir as cidades no mapa, pode estar configurando os algoritmos:
Selecione o algoritmo que deseja no canto esquerdo e Altere as configurações específicas daquele método conforme desejado.


	3. Execução e Resultado

Após configurar o algoritmo que deseja, basta clicar em Executar, no Mapa será gerado duas rotas: Rota inicial e Otimizada
O usuário pode estar exibindo qual deseja, clicando em cima de Rota inicial/Rota Otimizada.
No canto inferior será exibido em Resultado a distância Inicial, Distância Estimada(otimizada), cidades(pontos no mapa) e numero de interações conforme o algoritmo executado
Além de mostrar um grafico de custo do algoritmo

	4. Utilizando o botão "Análise de Algoritmo"

O botão de Análise comparativa. Ao clicar no botão, o sistema fará o seguinte fluxo automático:

Filtragem: Ele irá ler e filtrar todos os pontos (cidades) que você inseriu no front-end.

Execução: O programa executará todos os métodos de algoritmo no sistema de uma vez para aquele mesmo conjunto de cidades que foi definido.

Parâmetros: Durante essa execução em massa, o sistema vai rodar cada algoritmo conforme a configuração individual que foi deixada salva/selecionada para ele.

Resultados e Ganho: Ao final do processamento, será exibido uma interface mostrando o ganho de cada método. Isso permite que você compare qual algoritmo encontrou a melhor solução ou qual foi o mais eficiente para aquele cenário específico.