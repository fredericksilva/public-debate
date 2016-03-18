## Public Debate

### 1. Plugin para Debates
#### [1.1 Documentos Técnica](#)

- [1.1.1 Instalação / Desinstalação](#)

- [1.1.2 Descrição da base de dados](#)

- [1.1.3 Organização dos arquivos](#)

- [1.1.4 Descrição dos hooks, actions e filters utilizados](#)

### Lista de Actions
- [ 1.1.5 Descrição das funções do plugin](#)
- [ 1.2 Funcionalidades do Plugin ](#)
- [ 1.2.1 Cadastrar Debates Públicos]()
- [ 1.2.2 Listar Debates Públicos Cadastrados]()
- [  1.2.3 Estatísticas de Debates]()
- [1.2.4 Exportação de Debates]() ............15
- [1.2.5 Incorporar Debate a uma Página no Wordpress ](#)
- [1.2.6 Exibir Debate (Visão Pública)]()
- [1.3 Propostas de Evolução do plugin]()
- [1.3.1 Posicionamento]()
- [1.3.2 Ranking de Comentários e Trechos]()
- [1.3.3 Tipo do Comentários]()
- [1.3.4 Thread de Comentários]()
- [1.3.5 Moderação]()
- [1.3.6 Mídia dos comentários]()

#### 1 Plugin para Debates

Existe diversas formas de mobilizar comunidade online e por mais que
um texto de mais de duzentas páginas possa apresentar uma interação muito
diluída, existe a possibilidade de criar um espaço de debate online com tópicos
abordados na pesquisa.
Uma espécie de sumário de conceitos como o índice de um livro, que
serviria como um primeiro ponto de contato com o conteúdo, onde pessoas
poderiam debater livremente. Isto aconteceria em um universo de conteúdo
mais resumido do que a publicação proporcionando a concentração do
conteúdo. Com isto em mente surge a proposta de um plugin para wordpress.
O plugin Public Debate foi elaborado visando proporcionar uma rápida
criação de debates online. Estamos acompanhando um constante crescimento
da participação da sociedade civil em iniciativas de interação online.
Este plugin foi criado sobre a plataforma wordpress e em alinhamento
com as recomendações técnicas para o desenvolvimento avançado de plug-ins
acessível no website wordpress.org . Desta forma garante-se que atualizações
da plataforma não deveram afetar o funcionamento deste, assim como uma
manutenção mais fácil.
A seguir são apresentadas as principais característica técnicas do
plugin, a forma como foi construído e um breve manual de utilização.

#### 1.1 Documentação Técnica
<p>
O plugin, assim como a plataforma wordpress, é construído na
linguagem PHP e com banco de dados MySQL. O código-fonte do plugin está
disponibilizado na plataforma de codificação social github e também publicado
no site do wordpress (no atual momento aguarda aprovação)</p>
Este plugin está em uso apenas no portal Pensando o Direito, porém
está pronto para utilização em qualquer outro portal construído sobre a
plataforma wordpress.
A url de acesso ao projeto no github é:
[mobiwave/public_debate](https://github.com/mobiwave/public_debate). 
Github é uma ferramenta que funciona como repositório de código e encoraja o compartilhamento de
conhecimento. O repositório do projeto Public Debate está como público e não possui nenhuma licença associada ainda. Pelo fato do projeto estar em fase
beta e ser fruto de uma pesquisa, espera-se que este seja publicado sobre
licenças permissivas como MIT ou BSD caso este ganhe visibilidade.
Em diversas partes deste capítulo serão mencionadas funções. Estas se
referem a sequências de códigos executadas pela aplicação para realizar as
tarefas necessárias para o funcionamento do plugin. Uma função pode ser
entendida como uma engrenagem do motor enquanto o plugin se refere ao
motor inteiro

#### 1.1.1 Instalação / Desinstalação
<p>O procedimento de instalação deste plugin é o mesmo de qualquer outro
plugin criado para a plataforma wordpress. Basta que este seja colocado na
pasta “wp-content/plugins/” e depois seja ativado no painel administrativo do
wordpress.</p>
<p>
O plugin possui um script de instalação e desinstalação. Durante a
instalação (quando o plugin é ativado pela primeira vez) são criadas duas
tabelas no banco de dados, uma é responsável por armazenar os dados do
debate como um todo e outra para armazenar cada uma das partes
comentáveis.</p>
Para desinstalar o plugin basta utilizar a interface administrativa do
wordpress, navegar no item de menu plug-ins, desativá-lo e solicitar a
remoção.
É importante entender a diferença entre desativação e desinstalação,
enquanto a primeira mantém os dados da consultas cadastradas a segunda
exclui todo e qualquer arquivo do plugin, apagando inclusive todos os dados
dos debates. A instalação e desinstalação do plugin são executadas
respectivamente pelas funções: “public_debate_install()” e
“public_debate_uninstall()”.

### Importante

Este texto é parte de um relatório mais extenso desenvolvido
com outro propósito central e pode conter menções e referências a itens que
não se encontram neste documento. Quanto a isto peço desculpas.

## Duvidas
Dúvidas podem ser encaminhadas para [matheusneves@gmail.com](mailto:matheusneves@gmail.com)
<h3>Por favor, veja o arquivo README.pdf. Traduzi-lo para o MarkDown e transformá-lo no README oficial será um trabalho muito apreciado!</h3>
