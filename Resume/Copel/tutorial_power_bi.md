
## Microsoft Power BI
O Power BI é uma ferramenta de Business Intelligence (BI) que permite aos usuários visualizar e analisar dados de diferentes fontes, criar relatórios e dashboards interativos e compartilhar com outros usuários.


## Instalação
- Digite no prompt cmd:  ```ipconfig/ all```;
- Copie o código que aparece na opção "Nome do Host";
- Solicita um tolken e instalaram o software na sua  máquina.


## Filtros
Utilizar filtros para realçar os dados mais relevantes e utilizar recursos de formatação condicional para chamar atenção para valores específicos.
 - O filtro é aplicado à todos os gráficos e cartões presente no Dashboard;

## Tema
Um tema personalizado será aplicado somente no relatório atual, para aplicar em outros relatórios é necessário carregar novamente o tema personalizado.
 
Para criar um tema:
1. Acesse o Power BI Desktop e abra o relatório no qual deseja criar um tema personalizado.

1. Clique em "Formato" no menu superior, depois em "Tema atual" e escolha "Editar tema"

1. A janela de edição de tema será aberta, nele você pode editar as cores, fontes, efeitos e outros aspectos visuais do tema.

1. Quando terminar, clique em "Aplicar" para salvar as alterações.

Opcionalmente, você pode salvar o tema personalizado como um arquivo JSON clicando em "Salvar tema" e dando um nome para ele. Isso permitirá que você carregue o tema em outros relatórios no futuro.

 

Para utilizar um tema:

Barra de Menu -> Exibição -> Temas -> Clique para expandir os temas -> Procurar temas -> Selecione o arquivo JSON no seu computador -> o tema será aplicado automaticamente
 
## Modelagem de Dados
É o processo de criar uma representação visual ou esquemática, que define os sistemas de coleta e gerenciamento das informações de qualquer organização. Gerando um modelo que descreve quais dados foram coletados, a relação entre eles e os métodos usados para armazenar e analisar os dados.
 
Utilizar quando as informações em diferentes tabelas importadas para o Power BI se cruzam;
Finalidade, quando não há um relacionamento correto entre as tabela os gráficos gerados retornam valores errados;
Não é possível fazer relacionamentos com informações duplicadas;
Transformar dados ->Selecionar a coluna -> Botão Direito do mouse -> Remover duplicatas
O Power BI tenta fazer esses relacionamentos de forma automática, então é necessário conferir, apenas se as informações se cruzam, por exemplo, utilizar uma coluna da Tabela 1 como parâmetro do eixo X e uma coluna de outra tabela (Tabela2) como eixo Y.
Evite usar a cardinalidade muito para muitos, normalmente gera erros. Utilize as cardinalidades (1:1, 1:* ou *:1).
O Power BI não cria modelos (conceitual, lógico e/ou físico), o mesmo gera uma versão simplificada e geral, similar a um modelo lógico.
Você não consegue criar os relacionamentos entre as tabelas se os dados não estiverem corretamente conectados, entretanto permite a criação de gráficos e dashboards entre tabelas diferentes e resulta em valores errados.
O Power Bi tenta criar um modelo simplificado, para verifique ou modificar como é feito esses relacionamentos em Gerenciar relações.


## Importação de gráficos não nativos do Power BI
De outro modelo do Power BI, você pode seguir os seguintes passos:

Acesse o Power BI Desktop e abra o relatório em que deseja importar o gráfico.

Clique em "Visualizações" no menu superior e selecione "Importar visualização personalizada".

Selecione o arquivo do gráfico que deseja importar. Ele deve estar no formato .pbiviz.

Adicione os dados necessários para o gráfico e configure-o como desejado.

É importante verificar se o gráfico importado é compatível com a versão do Power BI que você está usando

 

De linguagens de programação, como R e Python:

Instale o pacote "plotly", ambas possui essa biblioteca.

Use o pacote para criar sua visualização personalizada e converta-a em um objeto JSON usando a função "toJSON()" do plotly.

Utilize a função "add_trace()" para adicionar a visualização personalizada no Power BI.

 

Como imagem:

Utilizando o recurso "Inserir Imagem" no Power BI Desktop, você pode adicionar uma imagem a partir de um arquivo local ou da internet.

Utilizando o recurso "Inserir Web Content" você pode adicionar um gráfico criado em outra ferramenta como por exemplo Excel, Google Sheets, entre outros.

Utilizando o recurso "Inserir URL" você pode adicionar uma imagem de uma url, por exemplo, se você tem uma imagem armazenada em um bucket na AWS ou Google Cloud Storage você pode adicionar ela pelo seu link.

Utilizando o recurso "Inserir HTML" você pode adicionar um gráfico criado em uma biblioteca javascript como D3.js, Chart.js, entre outros.

Ao importar uma imagem, ela não será dinâmica e não será possível modificá-lo.



## Data Analysis Expressions - DAX
Recomendações:
Preferencialmente utilizar as fórmulas das funções DAX, ao invés de fazer expressões diretamente nas colunas;
Há funções prontas em:
Dados -> Ferramentas da Tabela -> Medida Rápida -> Selecionar algum cálculo;


## Observações
O Power BI possui limite no carregamento de dados, pois o mesmo não é um banco de dados, para importar grande volume de dados integre com um banco de dados;

## Referências


