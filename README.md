<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com"&gt;>
    <link rel="stylesheet" href="assets/style.css">
    <link rel="preconnect" href="https://fonts.gstatic.com&quot; crossorigin>
    <link
        href="https://fonts.googleapis.com/css2?family=Bai+Jamjuree:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;1,200;1,300;1,400;1,500;1,600;1,700&display=swap&quot;
        rel="stylesheet">
    <title>Flashcards</title>
</head>

<body>
    <main>
        <section id="container">

            <article class="cartao">
                <div class="cartao-conteudo">
                    <h3>Matemática</h3>
                    <div class="cartao-conteudo-pergunta">
                        <p>Qual era a pessoa maisinteligente do mundo?</p>
                    </div>
                    <div class="cartao-conteudo-resposta">
                        <p>Albert Einsten </{p>
                    </div>
                </div>
            </article>

            <article class="cartao">
                <div class="cartao-conteudo">
                    <h3>Hístoria </h3>
                    <div class="cartao-conteudo-pergunta">
                        <p>Qual país ganhou a 2 Guerra Mundial</p>
                    </div>
                    <div class="cartao-conteudo-resposta">
                        <p>Foi o grupo dos aliados</p>
                    </div>
                </div>
            </article>

            <article class="cartao">
                <div class="cartao-conteudo">
                    <h3>Economia</h3>
                    <div class="cartao-conteudo-pergunta">
                        <p> Qual país tem a maior economia do mundo?</p>
                    <div class="cartao-conteudo-resposta">                 
                        <p>Estados Unidos</p>
                    </div>
                </article>

                <article class="cartao">
                    <div class="cartao-conteudo">
                        <h3>Matemática </h3>
                        <div class="cartao-conteudo-pergunta">
                            <p>Qual a raiz quadrada de 81?</p>
                        </div>
                        <div class="cartao-conteudo-resposta">
                            <p>9</p>
                        </div>
                    </div>
                </article>
                <article class="cartao">
                    <div class="cartao-conteudo">
                        <h3>Matemática </h3>
                        <div class="cartao-conteudo-pergunta">
                            <p>Qual a raiz quadrada de 9</p>
                        </div>
                        <div class="cartao-conteudo-resposta">
                            <p>3</p>
                        </div>
                    </div>
                </article>
                <article class="cartao">
                    <div class="cartao-conteudo">
                        <h3>Matemática </h3>
                        <div class="cartao-conteudo-pergunta">
                            <p>Qual a raiz quadrada de 144</p>
                        </div>
                        <div class="cartao-conteudo-resposta">
                            <p>12</p>
                        </div>
                    </div>
                </article>







                :root {
    --text-color: #4b6e99;
    --card-front-color: #021f06;
    --card-back-color: #64ec64;
}

body{
    background: url(https://thumbs.dreamstime.com/b/uma-pintura-multicolorida-que-cria-um-fundo-abstrato-din%C3%A2mico-para-design-de-wallpaper-hd-362994731.jpg);
    color: antiquewhite;
    font-family: bai-Jamjuree;
}

footer{
    background-color: rgb(63, 250, 73);
    color: rgb(20, 27, 32);
    position: fixed;
    bottom: 0;
    width: 100%;
    height: 2rem;
}
footer p{
    text-align: center;
    font-size: 0,7rem;
    margin-top: 0.5rem;
}

#container {
    display: flex;
     flex-wrap: wrap;
     justify-content: space-between;
     padding: 4rem;
     gap: 3rem;
}

.cartao {
    margin: 1rem 1rem;
    background-color: rgb(12, 62, 62);
    height: 20rem;
    flex-grow: 1;
    flex-basis: calc(33% - 6rem);
}

.cartao-conteudo {
    background-color: var(--card-front-color);
    text-align: center;
    height: 100%;
    transform-style: preserve-3d;
    transition: transform 300ms ease-in-out;
}

.cartao-conteudo h3 {
    color: var(--text-color);
    border: 1px solid var(--text-color);
    text-align: left;
    padding: 0.5rem;
    position: absolute;
    margin: 0.6rem;
    border-radius: 0.6rem;
    font-size: 1vw;
    backface-visibility: hidden;
}

.cartao-conteudo-pergunta p{
    color: var(--text-color);
    font-weight: 500;
}

.cartao-conteudo-resposta p{
    color: var(--card-back-color);
    font-weight: 700;
}

.cartao:hover .cartao-conteudo {
    transform: rotateY(180deg);
}

.cartao-conteudo-pergunta,
.cartao-conteudo-resposta {
    backface-visibility: hidden;
    position: absolute;
    height: 100%;
    width: 100%;
}

.cartao-conteudo-resposta {
    transform: rotateY(180deg);
}
.cartao-conteudo p {
    margin-top: 1rem;
    padding: 2rem;
    margin-top: 4rem;
}
