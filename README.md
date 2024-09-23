@import url('https://fonts.googleapis.com/css2?family=Krona+One&family=Montserrat:ital,wght@0,400;1,600&display=swap');

:root {
    --cor-primaria: #000000;
    --cor-secundaria: #F6F6F6;
    --cor-terciaria: #00D261;
    --cor-quartenaria: #54dd94;
    --cor-hover:#272727;
    --font-primaria: 'Krona One', sans-serif;
    --font-secundaria: 'Montserrat', sans-serif;
}
*{ /* reseta o tamanho/ layuot da pagina*/
    margin: 0;
    padding: 0;
}
body { /*corpo do texto */
    box-sizing: border-box;
    background-color: var(--cor-primaria);
    color: var(--cor-secundaria);
}
.cabecalho { 
    padding: 2% 0% 0% 15%;
}
.cabecalho__menu {
    display: flex;
    gap: 80px;
}
.cabecalho__menu__links {
    font-family: var(--font-secundaria);
    font-size: 1.5rem;
    font-weight: 600;
    color: var(--cor-terciaria);
    text-decoration: none;
    transition: 0.2s;
}
.cabecalho__menu__links:hover {
    color: var(--cor-quartenaria);
    transform: scale(1.1);
}
.imagem {
    width: 40%;
    border-radius: 10%;
    transition: 0.4s;
}
.imagem:hover { /* Animação hover imagem*/
    width: 43%;
    transform: scale(1.1);
}
.apresentacao { /* Main */
    padding: 5% 15%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 82px;
}
.apresentacao__curriculo { /* Main Curriculo*/
    padding: 5% 15%;
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    gap: 82px;
}
.apresentacao__conteudo { /* Section para criar um conteiner para formatação do Título e conteúdo do texto */
    width: 50%;
    display: flex;
    flex-direction: column;
    gap: 40px;
}
.apresentacao__conteudo__nome { /*Estilização titulos curriculo*/
    font-size: 1.85rem;
    font-family: var(--font-primaria);
    color: var(--cor-quartenaria);
}
.apresentacao__conteudo__titulo { /* Titulo (h1)*/
    font-size: 2.25rem;
    font-family: var(--font-primaria);
}
.titulo-destaque { /*Strong dentro de h1 (index)*/
    color: var(--cor-terciaria);
}
.apresentacao__conteudo__Descr { /* Estilização texto curriculo*/
    font-size: 1.25rem;
    font-family: var(--font-secundaria);
}
.apresentacao__conteudo__tabela { /*Estilização tabela curriculo*/
    padding: 1%;
}
.apresentacao__conteudo__texto { /*Texto (p)*/
    font-size: 1.5rem;
    font-family: var(--font-secundaria);
}
.apresentacao__links { /* Div conteiner para agrupar os botões das redes sociais*/
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    gap: 32px;
}
.apresentacao__links__subtitulo { /* h2 */
    font-family: var(--font-primaria);
    font-weight: 400;
    font-size: 1.5rem;
}
.apresentacao__links__botao { /* Estilização botões ancoras hiper links (a) */
    display: flex;
    justify-content: center;
    gap: 16px;
    border: 2px solid var(--cor-terciaria);
    width: 50%;
    font-weight: 600;
    padding: 21.5px 0;
    text-align: center;
    border-radius: 8px;
    font-family: var(--font-secundaria);
    font-size: 1.5rem;
    color: #f6f6f6;
    text-decoration: none;
    transition: 0.2s;
}
.apresentacao__links__botao:hover { /* Animação hover botão*/
    background-color: var(--cor-hover);
    padding: 3%;
    transform: scale(1.1);
}
.rodape {
    padding: 24px;
    background-color: var(--cor-terciaria);
    color: var(--cor-secundaria);
    text-align: center;
    font-family: var(--font-secundaria);
    font-size: 1.25rem; 
    font-weight: 400;
}
@media (max-width:1100px) {
    .cabecalho {
        padding: 10%;
    }
    .cabecalho__menu {
        justify-content: center;
        gap: 50px;
    }
    .imagem {
        width: 50%;
    }
    .apresentacao {
        flex-direction: column-reverse;
        padding: 5%;
    }
    .apresentacao__curriculo {
        flex-direction: column-reverse;
        padding: 5%;
        align-items: center;
    }
    .apresentacao__conteudo {
        width: auto;
    }
}
