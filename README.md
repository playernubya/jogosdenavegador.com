# jogosdenavegador.com

Joguinhos interativos para lives da Twitch com cara de computador dos anos 2000: cada jogo é um programa aberto numa área de trabalho estilo Windows 98 (o quiz **QI do Chat**, a palavra secreta, o caça-palavras, o **Detetive do Chat** e o fato ou fake), o chat responde digitando no chat, um apresentador zoa todo mundo e os pontos valem ranking do dia, do mês e geral.

**Um quadro criado por [PlayerNubya](https://twitch.tv/playernubya).**

Abra o link, digite o nome do seu canal e pronto. Não precisa criar conta, instalar nada nem cadastrar aplicativo.

---

## Como usar (3 passos)

1. **Abra o link do jogo** no computador e digite o nome do seu canal na Twitch.
2. **Copie o endereço** que aparece e cole no OBS numa fonte **Navegador** de **1920 × 1080**, com **Controlar áudio via OBS** marcado. O jogo ocupa a tela inteira, então use como uma **cena própria** do quadro.
3. **No chat**, digite `!qi` para começar.

Para testar antes da live, clique em **ver uma demonstração**: um chat falso joga sozinho.

O som **sempre começa no volume médio**, nunca no alto.

---

## Os jogos

| Jogo | Como o chat joga |
|---|---|
| **QI_DO_CHAT.EXE** | pergunta com 4 alternativas; o chat digita **A**, **B**, **C** ou **D** |
| **FATO_OU_FAKE.EXE** | curiosidade verdadeira ou inventada; o chat digita **V** ou **F**. Também aparece de surpresa no meio do QI |
| **PALAVRA.EXE** | palavra secreta de 4 a 8 letras (estilo Termo), com mais de 8 mil palavras e 23 temas; o chat chuta palavras e as letras ficam verdes ou amarelas |
| **CACA_PALAVRAS.EXE** | grade de letras com um tema; quem achar uma palavra escondida digita ela no chat |
| **DETETIVE.EXE** | cada rodada é um caso (10 cenas, cada uma com sua história) com 18 objetos camuflados em lugares sorteados; o jogo pede 7 pistas, uma por vez, e o chat digita a casa da grade (ex.: **C4**). A pista começa só com a sombra do objeto (vale 180), vira charada (140) e depois mostra o nome (100), com uma lanterna escurecendo parte da cena. Cada pessoa tem um chute por pista. No fim, o mural de polaroids mostra quem achou o quê e o detetive do dia. Tem trilha própria, um jazz noir |

Todos valem as mesmas **gemas** e o mesmo ranking. Quem quiser ver a própria posição digita **!pontos**.

### Comandos (dona do canal e moderadores)

| Comando | O que faz |
|---|---|
| `!qi` | começa uma rodada do QI (ou continua depois da pausa) |
| `!qi games` | escolhe o tema (lista abaixo) |
| `!qi fato` | próxima rodada só de fato ou fake |
| `!qi palavra` | abre a palavra secreta com tema sorteado; `!qi palavra games` escolhe o tema: animais, comidas, casa, natureza, corpo, games, brasil, filmes, esportes, profissoes, musica, escola, roupas, cores, paises, transportes, tecnologia, terror, festas, sentimentos, praia, natal, internet ou livre |
| `!qi caca` | abre o caça-palavras |
| `!qi detetive` | abre o Detetive do Chat |
| `!qi pausa` / `!qi pular` | pausa depois da pergunta atual / pula a atual (no Detetive, pula o objeto) |
| `!qi relampago` | a próxima pergunta vale o dobro |
| `!qi ranking` | mostra o ranking |
| `!qi fim` | encerra a rodada |
| `!qi descanso` | liga a proteção de tela na hora |
| `!qi abrir` / `!qi fechar` | mostra ou esconde a janela |
| `!qi som` / `!qi trilha` | desliga todos os sons / só a música |
| `!qi novalive` | começa um ranking "Hoje" novo |
| `!qi zerar hoje\|mes\|tudo` | zera o ranking escolhido (só a dona do canal) |

**Temas:** games, filmes, series, musica, brasil, historia, literatura, geek, ciencia, curiosidades, esportes, tv, memes, infancia, mitologia, geografia, leis, mix, fato.
**Subtemas:** dbd, cs, re, sh, tlou, minecraft, pokemon, nintendo, zelda, gta, lol, amongus, classicos, terror, marvel, disney, hp, starwars, nacional, sucessos, st, friends, got, animes, variadas, anos80, brasileira, rock, kpop.

---

## A área de trabalho

Os ícones funcionam com **dois cliques** (no OBS, clique com o botão direito na fonte → **Interagir**):

- **QI_DO_CHAT.EXE, PALAVRA.EXE, CACA_PALAVRAS.EXE, DETETIVE.EXE, FATO_OU_FAKE.EXE** abrem cada jogo
- **RANKING.DOC** mostra o ranking · **Temas** escolhe o tema da próxima pergunta
- **Música.mp3** liga e desliga a música · **Volume** alterna baixo, médio e alto
- **ajuda.txt** mostra os comandos · **Lixeira** guarda as respostas erradas da live

Detalhes da live: as fotos de quem errou voam para a Lixeira; quando ninguém acerta, aparece uma tela de erro fatal; o "chat da live" na barra de tarefas pisca quando alguém escreve; depois de alguns minutos sem rodada, entra a proteção de tela com o mascote quicando.

---

## Painel de controle

Abra o mesmo endereço com `?painel` no fim (ou o arquivo `painel.html`). No OBS, crie uma **segunda fonte de navegador** com esse endereço, deixe oculta e use pelo **Interagir**.

- **Controles:** iniciar, pausar, pular, relâmpago, ranking, encerrar, tema
- **Perguntas:** buscar, corrigir, desativar e criar as suas
- **Falas do apresentador:** desativar as que não combinam e criar as piadas internas do canal
- **Backup:** salvar e restaurar rankings, perguntas e configurações
- **Configurações:** tempos, volume, lado da janela, pontuação, proteção de tela (em minutos; 0 desliga), premiação

> Edições ficam guardadas no navegador onde você mexeu. O que você editar no Chrome **não** aparece no OBS. Para valer na live, use o painel dentro do OBS.

### Backup (não pule)

O ranking fica salvo dentro da fonte do OBS. Se o OBS limpar o cache, some tudo. No painel, em **BACKUP**, clique em **Gerar backup na caixa**, copie o texto e guarde num arquivo. Para restaurar, cole e clique em **Importar**.

---

## Recursos opcionais

### Premiar com pontos do canal (StreamElements)

No painel, cartão **NUBYACOINS**: pegue o **JWT Token** em streamelements.com → avatar → **Account** → **Show secrets**, cole no campo, clique em **Testar conexão** e salve.

> O token dá controle da sua conta do StreamElements. Não mostre o painel na live.

### Mascote

A apresentadora é a **Disquetinha**, um disquete com microfone desenhado pela PlayerNubya. O arquivo `mascote.gif` é a animação principal, e as expressões ficam em `mascote-feliz.gif`, `mascote-triste.gif`, `mascote-chocado.gif`, `mascote-dormindo.gif` e `mascote-pensando.gif`. Para usar outro mascote, troque os arquivos mantendo os nomes; as expressões são opcionais.

### Pontuação

No painel: **peso da velocidade** (0% = todo acerto vale igual), **janela de velocidade** e **penalidade por erro**. A velocidade conta a partir do primeiro acerto, para o atraso da Twitch não decidir quem ganha.

---

## Como colocar no ar (GitHub Pages)

1. Repositório público com estes arquivos na raiz: `index.html`, `painel.html`, `README.md`, `.nojekyll`, `mascote.gif` e as expressões `mascote-feliz.gif`, `mascote-triste.gif`, `mascote-chocado.gif`, `mascote-dormindo.gif`, `mascote-pensando.gif`, as cenas do Detetive `detetive-01.webp` a `detetive-10.webp` e os objetos `detetive-objetos.webp`
2. **Settings → Pages**: *Deploy from a branch*, a branch principal, pasta `/ (root)`
3. Para atualizar: **Add file → Upload files**, com o arquivo **exatamente** com o nome `index.html` (se o navegador baixou como `index (1).html`, renomeie antes), e **Commit changes**
4. Depois de 1 ou 2 minutos, recarregue com **Ctrl+F5**; no OBS, propriedades da fonte → **Atualizar cache da página atual**

---

## Perguntas frequentes

**Preciso de bot ou servidor?** Não. O jogo lê o chat sozinho, direto do navegador.

**Funciona em canal pequeno?** Sim. Com duas pessoas no chat já roda.

**No navegador o jogo ficou parado na abertura.** Ele espera o `!qi` no chat (a live não precisa estar ligada) ou o botão **▶ COMEÇAR**.

**Dá para pular a tela inicial?** Sim: acrescente `?canal=seunome` no fim do endereço.

**As fotos do chat não aparecem.** Elas vêm de um serviço externo gratuito; se ele cair, o jogo desenha avatares coloridos com a inicial.

---

## Créditos

Criado por **PlayerNubya** ([Twitch](https://twitch.tv/playernubya) · [TikTok](https://tiktok.com/@playernubya) · [Instagram](https://instagram.com/playernubya) · [YouTube](https://youtube.com/@playernubya)).

Cenas e objetos do Detetive do Chat desenhados pela PlayerNubya. Música e efeitos sonoros são gerados pelo próprio jogo (sem direitos autorais de terceiros). Fontes embutidas: **Jersey 10** e **VT323** (licença SIL Open Font). Palavras secretas: lista de frequência [wordfreq](https://github.com/rspeer/wordfreq) filtrada pelos dicionários **br.ispell** e **pythonprobr** (via [@andsfonseca/palavras-pt-br](https://github.com/andsfonseca/palavras-pt-br), licença MIT); filtro de palavrões da lista [toxibr](https://www.npmjs.com/package/toxibr) (licença MIT).

Se usar na sua live, deixe o crédito na tela e manda um alô. 💜
