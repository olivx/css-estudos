# Estudo para csss avançado.

#### curos: https://www.udemy.com/advanced-css-and-sass/

### gradient :
 - **exemplo:**

    background-image:
        linear-gradient(to right bottom,
        rgba(126,213,111,0.8),rgba(40,180,131,0.8))

        linear grandiente é a função em css para aplicar o gridente ,
        onde você passa as cores em rgba e o nivel de opacidade é opcional
        rgba(126,213,111,0.8), rgba(40,180,131,0.8) de verde claro para verde
        escuro com opacidade de 80%

    image que fica em baixo do gradiente url(../img/hero.jpg);

- cortar a div ou imagem
    clip-path: para cordar a imgem em formato específico:

    **exemplo:**
    clip-path: polygon(0 0, 100% 0 ,100% 80% ,0 100%)

- site para clip-path:
    esse site já varios formatos onde ele mostra a forma e deixa o codigo usado
    pela funcção polygon
    **polygon:** http://www.bennettfeely.com/clippy/

- centralizar div:
para centralizar uma div você deve colocar as laterais na metade do scren com top e left há 50% e usar o transform translate para ajustar.
O letf e top usa a x e y do meu viewport
tranform translate utiliza o top e left do elemente que esta na seleção em nosso caso a div text-box.
**Exemplo**

    ```css
    position: absolute;
    top: 40%; left: 50%;
    transform: translate(-50%, -50%)
    ```


- complexo efeito no botão:
movimento o botão durante o click e hover, e faz um fade no hover
**Exemplo**

    ```css
    .btn:link,
    .btn:visited {
        padding: 15px 40px;
        text-transform: uppercase;
        text-decoration: none;
        display: inline-block;
        transition: all .2s;
        border-radius: 100px;
        font-weight: 300;
        position: relative;
    }

    .btn:hover {
        transform: translateY(-3px);
        box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    }

    .btn:active {
        transform: translateY(-1px);
        box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
    }

    .btn-white{
        background-color: #fff;
        color: #777;
    }

    .btn::after {
        content: "";
        display: inline-block;
        height: 100%;
        width: 100%;
        border-radius: 100px;
        position: absolute;
        top: 0;
        left: 0;
        z-index: -1;
        transition: all .4s;
    }

    .btn-white::after {
        background-color: #fff;
    }

    .btn:hover::after {
        transform: scaleX(1.4) scaleY(1.6);
        opacity: 0;
    }

    .btn-animeted {
        animation: moveInBottom .5s ease-out .75s;
        animation-fill-mode: backwards;
    }
    /* animação no load da pagina */
    @keyframes moveInBottom {

        0% {
            opacity: 0;
            transform: translateY(30px)
        }
        100% {
            opacity: 1;
            transform: translateX(0)
        }
    }
```
