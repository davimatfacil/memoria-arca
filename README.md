# ⛵ A Arca de Noé - Jogo da Memória

Jogo da memória bíblico para crianças (pensado para 7 anos). Em cada fase a criança encontra os pares de animais, e eles "entram" na Arca. Ao fim de cada fase aparece uma curiosidade de Gênesis e uma pergunta rápida valendo uma estrela bônus.

## Como jogar

- **3 fases:** 4, 6 e 8 pares de animais.
- **Estrelas:** quanto menos jogadas, mais estrelas (de 1 a 3 por fase), mais 1 estrela bônus se acertar a pergunta.
- **Chuva:** diminui a cada fase e, ao salvar todos os animais, o céu clareia e aparece o arco-íris.
- **Som:** o botão 🔊/🔇 no topo liga e desliga os sons, e o navegador lembra a escolha.
- Funciona no celular, no computador e com teclado (Tab e Enter).

## Jogar online

Depois de publicar no GitHub Pages, o endereço fica assim:

`https://davimatfacil.github.io/memoria-arca/`

## Como publicar no GitHub Pages

1. No GitHub, crie um repositório novo chamado `memoria-arca`, marcado como **Public**.
2. Envie os arquivos `index.html` e `README.md` para a raiz do repositório (botão **Add file > Upload files**).
3. Vá em **Settings > Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**, branch **main** e pasta **/ (root)**, e clique em **Save**.
5. Espere cerca de 1 minuto e atualize a página. O endereço do jogo aparece no topo de **Settings > Pages**.

O nome do arquivo precisa ser exatamente `index.html`, porque é ele que o GitHub Pages abre por padrão.

## Como é feito

É um único arquivo HTML, sem biblioteca externa e sem imagem:

- **Embaralhamento:** algoritmo Fisher-Yates, que dá a mesma chance para toda ordem possível das cartas.
- **Sons:** gerados pelo navegador com a Web Audio API, só depois do primeiro toque (os navegadores bloqueiam som antes disso).
- **Pomba:** desenhada em SVG, para ser igual em todos os celulares.
- **Quiz:** as opções são embaralhadas com Fisher-Yates, marcando a correta antes do sorteio, para a resposta não ficar sempre na mesma posição.
- **Acessibilidade:** cartas e botões funcionam com teclado e a animação é reduzida para quem desativa movimento no aparelho.

## Textos bíblicos

Os versículos mostrados ao fim de cada fase (Gênesis 6:14, 7:9, 8:11 e 9:13) são citados da Nova Versão Transformadora (NVT), da Editora Mundo Cristão, sempre com a referência. Os direitos do texto pertencem à editora.
