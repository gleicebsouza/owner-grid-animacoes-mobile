- {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }
  /_root : sudo elements
  62.5 % = 10 px
  _/
  :root {
  --hue: 250;
  --primary-color: hsla(232, 17%, 35%, 1);
  --second-color: hsla(218, 17%, 62%, 1);
  --tree-color: hsla(275, 18%, 79%, 1);
  --four-color: hsla(312, 91%, 96%, 1);
  --six-color: hsla(233, 100%, 97%, 1);
  --seven-color: hsla(274, 84%, 12%, 1);

  font-size: 62.5%;
  --f-heading: clamp(4rem, 1rem + 5vw, 5.6rem);
  --fs-heading2: clamp(3rem, 0.5rem + 3vw, 4rem);
  }
  body {
  border: 1px solid rgb(125, 5, 5);

  background-color: hsla(233, 100%, 97%, 1);
  }
  .page {
  width: 38rem;

  margin: 0 auto;
  border: 2px solid rgb(165, 6, 123);
  }

main {
margin: 0 auto;
animation: downtop 700ms 350ms backwards;
}

#logo {
margin-top: 1.8rem;
}
img {
margin: 0 auto;
transition: transform 1s 200ms ease-in;
}
img:hover {
transform: scale(1.1);
}

.title::before {
background-color: hsla(218, 17%, 62%, 1);
width: 100%;
height: 27.9rem;

content: '';
position: absolute;
top: 0;
left: 0;
z-index: -1;
margin: 0 auto;
}
.page header {
position: relative;
display: flex;
flex-direction: column;
align-items: center;
}
header {
font-family: 'Staatliches', cursive, sans-serif;
align-items: center;
margin: 0 auto;
animation: topdown 700ms backwards;
}
main,
section p {
font-family: 'Palanquin', sans-serif;
}
.title {
background: var(--tree-color);
height: 4.9rem;
width: 100%;
display: inline-flex;
justify-content: center;
align-items: center;

padding: 0.8rem 8.6rem;
cursor: pointer;
border: 1px solid rgb(125, 5, 5);
}
.title h1 {
align-items: center;
color: white;
font-family: 'Staatliches', sans-serif;
font-size: 3.8rem;
font-weight: 400;
line-height: 3.4rem;
letter-spacing: 0.05em;
transition: transform 2s 200ms;
}
.title h1:hover {
transform: scale(0.9);
}
.loren {
margin-top: 4rem;
}
.loren p {
color: var(--seven-color);
font-family: 'Palanquin';
font-weight: 400;
font-size: 2rem;
line-height: 1.5rem;
display: flex;
align-items: center;
text-align: center;

margin-bottom: 6.3rem;
padding: 1.4rem 3.6rem;
}
.images img {
border: 2px solid red;
object-fit: cover;
height: auto;
border-radius: 2rem;
filter: brightness(0.8);
margin-inline: 3.2rem;
}
.images {
position: relative;
///transition: all 1s 100ms ease-in;
}
.images:hover {
//transform: scale(1.1);
//opacity: 0.9;
}
.img-ice-cream {
display: grid;
gap: 3.2rem;
object-fit: cover;
}
.img-ice-cream h3 {
background-color: hsla(312, 91%, 96%, 1);
color: hsla(232, 17%, 35%, 1);

font-family: 'Staatliches';
font-weight: 400;
font-size: 2rem;
line-height: 3.4rem;
letter-spacing: 0.05em;

display: flex;
justify-content: center;
width: 11.2rem;
height: 3.5rem;

position: absolute;
top: 1rem;
right: 3.6rem;

border-radius: 2rem;
cursor: pointer;
}

@media (min-width: 1200px) {
.page {
width: 100%;
display: flex;
}
header {
width: auto;
}
.title {
width: 377px;
font-size: 2.6rem;
}
.title::before {
background-color: hsla(218, 17%, 62%, 1);
width: 377px;
height: 720px;

    content: '';
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    z-index: -1;
    margin: 0 auto;

}
.loren p:nth-child(1) {
position: absolute;
left: 0;

    height: 262px;
    width: 377px;
    border: 1px solid darkblue;

}
main {
grid-template-columns: 1fr 1fr;
}
}

/\*
---- regras de animações AT-RULES ----
at-rules:Keyframes,media

keyframes= pontos chaves na aplicação

@keyframes topdown {
0% {
opacity: 0;
transform: translateY(-15px);
}
100% {
opacity: 1;
transform: translateY(0);
}
}
@keyframes downtop {

100% {
opacity: 1;
transform: translateY(10px);
}
}
\*/
