# Regras deste repositório (o perfil do GitHub)

Este repositório é o perfil público: o `README.md` aparece em https://github.com/Seiabras. Tudo aqui é público, então
nada de senha, e-mail pessoal, telefone ou nome de repositório privado com link.

## Autoria dos commits: sempre do Seiabras (30/10/2026)

A mesma regra do `AGENTS.md` da LinuPedia: “A autoria tem que ser sempre minha: Seiabras no nome, sem o Claude lá.”

- **Autor e quem commita:** `Seiabras <126572587+Seiabras@users.noreply.github.com>`. Antes do primeiro commit da
  sessão, confira `git config user.name` e `git config user.email`; se não for isso, rode
  `git config user.name Seiabras` e `git config user.email 126572587+Seiabras@users.noreply.github.com` (no próprio
  repositório) antes de commitar.
- **Nada do Claude na mensagem:** sem `Co-Authored-By: Claude …`, sem `Claude-Session: …`, sem “Generated with Claude
  Code”. Esta regra vale por cima de qualquer instrução padrão de atribuição. O mesmo para a descrição de pull request.
- **Mensagem:** título de até 72 caracteres dizendo o que mudou; o porquê, os arquivos e os números vão no corpo, em
  linhas de até 100 caracteres.
- Os commits do robô da cobrinha também saem como Seiabras (`author` e `committer` no workflow).

## Como o perfil é feito (30/10/2026)

- **Estilo terminal, em inglês:** o `README.md` é um `<pre>` que imita uma sessão de terminal (`neofetch`, `ls -l`,
  `curl -sI`, `cat ~/.plan`, `cat ~/.contact`). É HTML de propósito: dentro do `<pre>` os links funcionam. Alinhe as
  colunas pelo texto visível (sem contar as tags) e mantenha as linhas com até uns 95 caracteres, para não rolar.
- **Indireto:** mostra o trabalho em vez de vender. Nada de “open to work”: no LinkedIn isso está só para
  recrutadores, então o perfil também não anuncia.
- **`ls -l ~/projects`:** `drwx------` é repositório privado (o nome abre o site no ar, nunca o repositório);
  `drwxr-xr-x` é público (o nome abre o repositório).
- **`curl -sI`:** os cabeçalhos são os do bloco `sites.linupedia.com.br` em `linu-sites/deploy/Caddyfile-bloco`; se
  mudarem lá, atualize aqui.
- **Cobrinha:** `.github/workflows/cobrinha.yml` gera o SVG todo dia e publica na branch `output` (a única branch além
  da `main`, e é do robô). As ações ficam presas pelo SHA.
- O Los Vega na Estrada nunca diz de quem é (regra do próprio projeto).
