Estudo para csss avançado.  
curos: https://www.udemy.com/advanced-css-and-sass/


gradient :
exemplo:

background-image:
linear-gradient(to right bottom,
rgba(126,213,111,0.8), rgba(40,180,131,0.8))

linear grandiente é a função em css , 
rgba(126,213,111,0.8), rgba(40,180,131,0.8)
de verde claro para verde escuro com opacidade
de 80% 


image que fica em baixo do gradiente 
url(../img/hero.jpg);

clip-path: para cordar a imgem em formato específico
clip-path: polygon(0 0, 100% 0 ,100% 80% ,0 100%)

site para clip-path: polygon:
http://www.bennettfeely.com/clippy/

centralizar:
para centralizar uma div você deve colar as laterais na metade do scrren com top e lieft a 50%
e usar o transform translate para ajustar com - 50% do tamanaho dela , quanto letf e top usa
a x e y do meu viewport o tranform translate utiliza do elemente que esta na seleção no caso
a div text-box.  

position: absolute;
top: 40%;
left: 50%;
transform: translate(-50%, -50%)



