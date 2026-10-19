# 📺 TV da Infância

Uma TV de tubo antiga que roda no navegador, feita para matar a saudade do tempo em que assistir TV não tinha preocupação nenhuma.

Gire o botão, ouça o chuvisco entre um canal e outro e deixe a programação rolar.

## O que ela tem

- **Visual de TV de tubo:** gabinete de madeira, tela curva, linhas de varredura, brilho de vidro e LED de ligado.
- **Botão de canal giratório** com chuvisco e ruído a cada troca.
- **Canais de exemplo** feitos do zero: barras de cor com bipe, desenho animado, jornal com letreiro rolando, vinheta de sessão de filmes e fim da programação.
- **Programe seus canais:** cole o link de uma playlist ou vídeo do YouTube em qualquer um dos 12 canais.
- **Meus vídeos:** carregue arquivos do seu aparelho e eles viram canais extras. Nada é enviado para a internet.
- **Controle de volume** e atalhos de teclado (← → ↑ ↓ trocam de canal).
- **Seus canais ficam salvos** no navegador.

## Como usar

1. Clique em **Ligar**.
2. Gire o botão ou toque nos números para mudar de canal.
3. Clique em **Programar canais**, cole o link de uma playlist do YouTube em um canal e aperte Enter.
4. Clique em **Ver** para sintonizar o canal.

## Rodando no seu computador

Não precisa instalar nada, é um único arquivo `index.html`.

O YouTube só libera o player em páginas com endereço web de verdade. Abrir o arquivo com duplo clique (`file://`) causa o **erro 153**. Rode com um servidor local:

```bash
python3 -m http.server 8000
```

Depois abra `http://localhost:8000`.

## Publicando na internet

Funciona em qualquer hospedagem de site estático:

- **Vercel:** importe o repositório em vercel.com/new e clique em Deploy.
- **Netlify Drop:** arraste o `index.html` em app.netlify.com/drop.
- **GitHub Pages:** ative o Pages nas configurações do repositório.

O arquivo precisa se chamar `index.html` e ficar na raiz do projeto.

## Problemas comuns

| Problema | O que fazer |
| --- | --- |
| Erro 153 no YouTube | Abra por `https://` ou `http://localhost`, nunca direto pelo arquivo. |
| O vídeo mostra aviso do YouTube | O dono do vídeo bloqueou a exibição fora do YouTube. Troque por outro. |
| Sem som no primeiro canal | O navegador só libera áudio depois do primeiro clique. Clique em Ligar. |

## Tecnologias

HTML, CSS e JavaScript puro, sem frameworks e sem dependências. Os efeitos visuais usam `canvas` e o som de chuvisco usa Web Audio API.

## Aviso

Este projeto não hospeda nem distribui nenhum programa de TV. Os vídeos tocam pelo player oficial do YouTube ou vêm dos arquivos do próprio usuário.

---

Feito com carinho e muita nostalgia. 🌈
