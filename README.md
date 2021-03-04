# netflix-clone
Recriando a página da Netflix
Neste projeto utilizamos nosso conhecimentos de css , HTML e javascript para recriar um front-end semelhante ao da gigante do streaming Netflix

![Uploading image.png…]()![Uploading image.png…]()



Clone do Netflix
Neste projeto , desenvolvemntos uma front-end idêntica a da Netflix .
Aprendemos conceitos sobre CSS , HTML5 e Javascritp
Utilizamos a extensão Live Server do Vs code para visualizar em tempo real as alterações feitas no navegador .
Usamos também a extensão auto rename tag para que ao modificar uma tag a de fechamento também seja modificiada
dica: Escrever html. faz surgir a opção html5 que ao ser clicada formnece a estrutura padrão do html
tags são divs , logo header , footer , etc são divs
alt + shift + para baixo clona a linha
webkits - aumentam a compatibilidade do css
sempre resetar o css antes de começar um site
 *{
    margin:0;
    padding:0;
    box-sizing: border-box;
}
declarando variaveis no css bom para declarar as cores principais do site

:root{
    --vermelho:#E50914;
    --preta:#141414;
}
google fonts contem fontes externas para seu projeto

flex box alinha os elementos em tela

row é a propriedade padrao

Melhora o contraste do texto

 background: linear-gradient(rgba(0,0,0,.50),rgba(0,0,0,.50)100%),  url('../img/capa-house.jpg');
Para renderizar o botao da maneira correta independete da plataforma

display : flex; joga os elementos para linha

flex-direction: column ; altera para coluna -justify context sempre segue a direção do flex direction -align-items: flex-start; alinha pel inicio (a esquerda) do flex column

uma div filha (que nao é principal, ou seja não é filha direta de um elemento que foi definido como flex) vem criada por padrão com display: block;

https://fontawesome.com/ site para buscar icones , atraves de um js , basta adinicionar o link que ele envia e vc jah pode adicionar o html do icone <script src="https://kit.fontawesome.com/2c36e9b7b1.js"></script>

pading cima baixo

pading cima direita baixo esquerda

.botao:hover para mudar a pintura quando passa o mouse

dentro de botao transition: .3s ease all; dura 3 segundos

icone do botao

 <div class="botoes">
                    <button role="button" class="botao">
                        <i class="fas fa-play"></i>
                        ASSISTIR AGORA
                    </button>
                    <i class="fas fa-info-circle"></i>
 </div>
classes wrapper
São classes que envelopam um conteúdo para que os filhos de primeiro grau herdem características

dessa forma vocÊ pode jogar tudo para esquerda ou direita movendo apenas o wrapper

dessa forma vocÊ pode por exemplo alinha o texto e o titulo sempre se os dois dependerem da classe container por exemplo

.filmeprincipal container afeta somente o que está dentro de filme principal e container -plugin jquery (está entrando em desuso) mas é bom pra aprender a usar

https://owlcarousel2.github.io/OwlCarousel2/

baixar a pasta do owl carrousel

criar uma pasta para o plugin wx: owl

na pasta docs -> assets -> vendors -> jquery.min

transferir para a pasta owl criada

docs -> assets -> owlcarousel -> owl.carousel.min (versao minificada do carousel)

transferir para a pasta owl criada

transferir para pasta owl criada >

owl -> dist -> assets -> owl.carousel.min e ownl.theme .default.min.css

<meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <link rel="stylesheet" href="style/main.css">

   <!--responsividade-->
   <link rel="stylesheet" href="style/responsive.css">

   <!--owl css-->
   <link rel="stylesheet" href="style/owl/owl.carousel.min.css">
   <link rel="stylesheet" href="style/owl/owl.theme.default.min.css">
o js deve ser sempre a ultima coisa a ser carregada na pagina

    <script src="https://kit.fontawesome.com/2c36e9b7b1.js"></script>
    <script src="js/owl/jquery.min.js"></script>
    <script src="js/owl/owl.carousel.min.js"></script>
    <script src="js/owl/setup.js"></script>
 

Pegando todo o tamanho

.box-filme{
    height: 100%;
    width: 100%;
    display: block;
    cursor: pointer;
}
parte 8
Aplicando estilos dependendo do tamanho da tela
máx 700 px joga pra baixo o botao quando a tela for 700 px
fornece uma margem top para nao ficarem tao grudados quando a tela diminuir
@media screen and (max-width:700px){
    header .container{
    display: flex;
    flex-direction: column;
    }

    .botao{
        margin-top: 5px;
        width: 300px;
    }

}
- min 1000px 700 px 
- descrição ocupa só 50 % da tela 
@media screen and (min-width:1000px){
    .descricao{
        width: 50%;
    }
}
cursor: pointer;
muda o cursor em cima do objeto
