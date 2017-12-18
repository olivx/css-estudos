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