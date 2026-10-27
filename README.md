Power BI Full Screen Dashboard
📌 Sobre o projeto

Este projeto consiste em uma página HTML desenvolvida para exibir dashboards do Microsoft Power BI em tela cheia, utilizando um iframe para incorporar o relatório por meio de um link público.

O layout foi configurado para ocupar 100% da largura e da altura da janela do navegador, sem margens externas e com ajustes de posicionamento para ocultar partes indesejadas da interface do relatório.

🚀 Funcionalidades
Tela cheia: ocupa 100% da largura e da altura da janela do navegador.
Sem margens externas: remove as margens e o espaçamento padrão da página.
Ocultação visual da barra inferior: o iframe possui altura adicional de 63 px para ultrapassar o limite inferior do contêiner.
Ajuste horizontal: utiliza margens e largura adicional para compensar pequenas bordas laterais.
Fundo preto: evita espaços brancos ao redor do dashboard.
Configuração simplificada: basta inserir o link público do Power BI na propriedade src.
⚙️ Configuração do dashboard

No arquivo HTML, localize a propriedade src do iframe:

HTML
<iframe
    src=""
    allowfullscreen>
</iframe>


Insira o link público do relatório Power BI no campo src.

Exemplo:

HTML
<iframe
    src="https://app.powerbi.com/view?r=SEU_LINK_PUBLICO"
    allowfullscreen>
</iframe>


Substitua SEU_LINK_PUBLICO pelo endereço real gerado pelo Power BI.

🖥️ Ajustes de layout

O CSS contém configurações específicas para adaptar o relatório à tela:

Propriedade	Finalidade
width: 100vw	Ocupa toda a largura da janela.
height: 100vh	Ocupa toda a altura da janela.
margin: 0	Remove as margens padrão da página.
overflow: hidden	Impede a exibição de barras de rolagem externas.
margin-left: -3px	Desloca o relatório 3 px para a esquerda.
width: calc(100% + 7px)	Adiciona 7 px à largura do iframe.
height: calc(100% + 63px)	Adiciona 63 px à altura para cortar visualmente a parte inferior.
border: none	Remove a borda do iframe.
▶️ Como executar
Salve o código em um arquivo chamado index.html.
Copie o link público do dashboard no Power BI.
Cole o link no atributo src do iframe.
Salve o arquivo.
Abra o index.html em um navegador para visualizar o dashboard.

Para disponibilizar o dashboard para outras pessoas, publique o arquivo HTML em um serviço de hospedagem web estática.

⚠️ Observações importantes
O ajuste de 63 px é um recorte visual da parte inferior do iframe; ele não desativa a barra inferior dentro do Power BI.
Os valores de margem, largura e altura podem precisar de ajustes conforme a resolução da tela e a interface do relatório.
A remoção das barras depende do tipo de link e dos parâmetros de incorporação suportados pelo Power BI.
O link de Publicar na Web torna o relatório acessível publicamente. Não utilize esse método para dados confidenciais ou restritos.
🛠️ Tecnologias utilizadas
HTML5
CSS3
Microsoft Power BI
iframe para incorporação do relatório
📄 Licença

Defina uma licença de acordo com as condições de uso e distribuição do projeto.
