My Heart to You 💖
Este projeto exibe um coração animado pulsante feito puramente com HTML e CSS. Ele é ideal para aprendizado ou como uma pequena demonstração de animação baseada em keyframes.

🎨 Descrição do Projeto
O coração animado é renderizado em uma página centralizada com o seguinte comportamento:

Um coração estilizado em vermelho com uma leve sombra.
A animação faz o coração pulsar, alternando entre tamanhos para criar um efeito visual de batimento cardíaco.
🛠️ Tecnologias Utilizadas
HTML: Estrutura da página e posicionamento do coração.
CSS: Estilização, animação e efeitos visuais.
🚀 Como Rodar o Projeto
Clone o repositório ou copie o código.
Certifique-se de que os arquivos index.html e style.css estejam no mesmo diretório.
Abra o arquivo index.html em qualquer navegador moderno.
📝 Código CSS Explicado
1. Estilização Geral
css
Copiar código
body {
    margin: 0;
    padding: 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #0b1522;
}
Remove margens e preenchimento padrão.
Define uma altura mínima de 100% da viewport.
Centraliza o conteúdo vertical e horizontalmente.
Define o fundo como azul escuro.
2. O Coração
css
Copiar código
.heart {
    height: 70px;
    width: 70px;
    background: #f20044;
    position: relative;
    transform: rotate(-45deg);
    box-shadow: -10px 10px 90px #f20044;
    animation: heart 0.6s linear infinite;
}
O coração é criado com um quadrado rotacionado a -45°.
box-shadow adiciona brilho ao redor.
animation utiliza keyframes para criar o efeito de pulsação.
3. Adicionando as Metades do Coração
css
Copiar código
.heart:before, .heart:after {
    content: '';
    position: absolute;
    height: 70px;
    width: 70px;
    background: #f20044;
    border-radius: 50px;
    box-shadow: -10px -10px 90px #f20044;
}
:before: Uma semicirculação posicionada no topo.
:after: Outra semicirculação posicionada na direita.
Ambas são arredondadas com border-radius.
4. Animação (Keyframes)
css
Copiar código
@keyframes heart {
    0% {
        transform: rotate(-45deg) scale(1.07);
    }
    80% {
        transform: rotate(-45deg) scale(1.0);
    }
    100% {
        transform: rotate(-45deg) scale(0.8);
    }
}
0%: Início da pulsação, o coração fica ligeiramente maior.
80%: Volta ao tamanho original.
100%: Contrai levemente para o efeito de batimento.
📂 Estrutura de Arquivos
bash
Copiar código
/my-heart-to-you/
├── index.html       # Estrutura HTML
└── css/
    └── style.css    # Estilização e animação do coração
🌟 Demonstração
Abra o arquivo index.html para visualizar o coração pulsante animado. 💓

📜 Licença
Este projeto é livre para uso e modificação. Sinta-se à vontade para personalizá-lo! 😊






