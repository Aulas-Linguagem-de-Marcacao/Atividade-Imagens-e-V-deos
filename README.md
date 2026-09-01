# Instrutivo do Aluno — Impressão 3D em Metal

**Situação-problema:** a empresa fictícia **MétricaTech**, fabricante de componentes industriais, deseja lançar uma página institucional para apresentar a sua nova linha de **impressão 3D em metal**. Os desenvolvedores da empresa já deixaram o conteúdo pronto, mas as **imagens e os vídeos ainda estão sem configuração visual** e a página está "crua" visualmente.

**Seu papel:** você foi contratado(a) como analista de front-end para entregar essa página. Deverá **estilizar as imagens e os vídeos** (tamanho, bordas, autoplay, etc.) e garantir que a página funcione corretamente no navegador.

**Regras:**

- Você pode usar a internet para pesquisar na **documentação oficial** (MDN, W3C, WHATWG) — <https://developer.mozilla.org>.
- **NÃO pode usar ferramentas de IA** (ChatGPT, Copilot, Gemini etc.).
- **NÃO deve copiar conteúdos prontos**; a solução deve ser escrita por você.
- Vocês devem pesquisar na internet as imagens relacionadas ao tema, salvar estas imagens dentro do diretório **imagens** e utilizar no projeto.
- Os vídeos devem ser linkados diretamente do YouTube ou qualquer outra plataforma de vídeo.

**Instruções:**
Faça o fork deste repositório para sua conta do GitHub, logo em seguida, faça o clone do repositório criado em sua conta para o seu computador.
Ao final da atividade fazer o versionamento e entregar o link no Google Classroom.

---

## Objetivos da atividade

Ao final, a página `index.html` da pasta `impressao-metal/` deve apresentar:

- [ ] **10+ imagens** sobre o tema, todas estilizadas (tamanho, bordas, arredondamento etc.).
- [ ] **1 imagem mapeada** (tags `<map>` e `<area>`) em que o clique em regiões leva a seções da página.
- [ ] **2 vídeos** com configurações adequadas (controles, loops, se aplicável `autoplay`/`muted`).
- [ ] Página responsiva e visualmente agradável.
- [ ] Todos os textos `alt` preenchidos corretamente (acessibilidade).

---

## Estrutura da pasta

```
impressao-metal/
├── imagens/          (arquivos de imagem do tema)
├── index.html        (página a ser completada e estilizada)
└── justificativa.txt (entregável — explique cada escolha)
```

---

## Passo 1 — Conheça o arquivo

Abra `index.html` no editor. A estrutura já está montada com:

- Cabeçalho, navegação, seções e rodapé estilizados.
- Área reservada para as imagens, vídeos e a imagem mapeada.

Preste atenção aos comentários com a palavra **MARCA** — eles indicam exatamente onde você deve intervir.

---

## Passo 2 — Estilize as imagens e os vídeos

No `<style>` da página você encontrará as classes:

| Classe | Onde se aplica | O que costuma configurar |
|--------|----------------|--------------------------|
| `.img-amostra` | todas as imagens | `width`, `height`, `border`, `border-radius`, `margin` |
| `.video-amostra` | todos os vídeos | `width`, `height`, `border`, `border-radius`, `margin` |

**Para as imagens você deve:**

- Definir `width` (e `height` quando necessário) para padronizar.
- Configurar `border` e/ou `border-radius` para um visual mais refinado.
- Garantir que todas as imagens tenham `alt` descritivo.

> **Desafio (pesquise na documentação):** use `object-fit: cover` para que as imagens não fiquem distorcidas quando tiverem largura/altura fixas.

**Para os vídeos você deve:**

- Definir `width`/`height`.
- Manter `controls` e configurar `loop` e `muted`.
- Aplicar, quando fizer sentido, `autoplay` e `poster` (imagem de capa).

---

## Passo 3 — Complete a imagem mapeada

Já existe uma imagem mapeada (`fluxo-metal.jpg`) com a tag `<map>`. Verifique as coordenadas dos `<area>` e ajuste se necessário para que:

- Cada região clique leve à seção correspondente (`#tecnologias`, `#aplicacoes`, `#galeria`, `#vantagens`).
- As regiões fiquem sobre áreas coerentes da imagem.

> **Dica (documentação):** pesquise sobre os atributos `shape` e `coords` da tag `<area>`.

---

## Passo 4 — Teste e revise

Abra `index.html` no navegador (duplo clique) e verifique:

- [ ] As imagens aparecem e estão bem dimensionadas.
- [ ] O clique na imagem mapeada leva às seções corretas.
- [ ] Os vídeos tocam e repetem (e, se configurado, iniciam automaticamente).
- [ ] A página fica boa em uma janela pequena (responsividade).
- [ ] Os textos `alt` descrevem corretamente cada mídia.

---

## Passo 5 — Entregue

- Versione o projeto **completo** (pasta `impressao-metal/`).
- Preencha o arquivo **justificativa.txt** explicando, para cada imagem/vídeo:
  - qual é o arquivo;
  - qual configuração você aplicou (tamanho, borda, etc.);
  - por que essa configuração foi escolhida.

---

## Critérios de avaliação

<table>
<thead>
<tr>
<th>Capacidade</th>
<th>Critério de avaliação</th>
<th>Alcançado</th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="5">Utilizar linguagem de marcação para desenvolvimento de páginas web</td>
<td><font color="red">(C) O aluno utilizou as tags de imagem seguindo os padrões da W3C?</font></td>
<td></td>
</tr>
<tr>
<td><font color="red">(C) O aluno utilizou tags de vídeos seguindo os padrões da W3C?</font></td>
<td></td>
</tr>
<tr>
<td><font color="red">(C) O aluno integrou vídeos de plataformas online na página, usando configurações adequadas para reprodução automática e em loop?</font></td>
<td></td>
</tr>
<tr>
<td>(D) O aluno configurou a tag de imagem pensando em acessibilidade e possíveis problemas no carregamento da imagem?</td>
<td></td>
</tr>
<tr>
<td>(D) O aluno conseguiu utilizar uma imagem mapeada fazendo acessos internos à página web?</td>
<td></td>
</tr>
<tr>
<td rowspan="3">Demonstrar pensamento analítico</td>
<td><font color="red">(C) O aluno salvou as imagens no diretório específico dentro do projeto?</font></td>
<td></td>
</tr>
<tr>
<td>(D) O aluno utilizou formatos de imagem compatíveis com os padrões da web?</td>
<td></td>
</tr>
<tr>
<td>(D) O aluno avaliou a estrutura atual do projeto, fazendo alterações pontuais apenas onde necessário?</td>
<td></td>
</tr>
<tr>
<td rowspan="2">Demonstrar autonomia</td>
<td><font color="red">(C) O aluno utilizou a documentação oficial (W3C e MDN) quando necessário para utilizar ou configurar uma tag?</font></td>
<td></td>
</tr>
<tr>
<td>(D) O aluno compreende a solução que ele mesmo implementou, respondendo perguntas pontuais dos professores?</td>
<td></td>
</tr>
</tbody>
</table>
(C) - Critérios Críticos <br>
(D) - Critérios Desejáveis
