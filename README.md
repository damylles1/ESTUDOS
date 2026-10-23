# Estudos da Ingryd

Site pessoal de estudos de Medicina: resumos por disciplina e assunto, banco de questões interativo e revisões espaçadas pelo desempenho.

O site inteiro está em um único arquivo: `index.html`. Os dados (disciplinas, questões, progresso e arquivos) ficam no Supabase, protegidos por login.

## Publicar pela primeira vez

1. **GitHub:** abra o repositório `estudos` → **Add file** → **Upload files** → envie o `index.html` (e este `README.md`) → **Commit changes**.
2. **Netlify:** **Add new site** → **Import an existing project** → **GitHub** → escolha `estudos`. Deixe os campos de build em branco e clique em **Deploy**.
3. Em **Site configuration** → **Change site name**, troque o nome para algo como `estudosdaingryd`. O endereço fica `https://estudosdaingryd.netlify.app`.
4. **Supabase:** em **Authentication** → **URL Configuration**, coloque o endereço do Netlify em **Site URL**. Assim o link do e-mail de confirmação volta para o seu site.
5. Abra o site, clique em **Primeira vez? Criar conta**, confirme pelo e-mail e entre.
6. **Importante:** depois de criar a sua conta, vá no Supabase em **Authentication** → **Sign In / Providers** e desligue **Allow new users to sign up**. Assim ninguém mais consegue criar conta no seu site.

## Editar o design

Toda mudança salva no GitHub atualiza o site em cerca de 1 minuto.

1. No GitHub, abra `index.html` e clique no lápis (**Edit**).
2. No topo do arquivo há a área **PERSONALIZE O VISUAL AQUI**:
   - `--accent` é a cor principal (botões, abas, destaques).
   - `--bg` é o fundo da página; `--surface` é o fundo das listas e cartões.
   - `--c1` a `--c8` são as cores disponíveis para as disciplinas.
   - `--f-display`, `--f-body` e `--f-mono` são as fontes. Para trocar, escolha outra em fonts.google.com e atualize também o `<link>` de fontes no topo.
   - `--r` controla o arredondamento dos cantos e `--largura` a largura máxima do conteúdo.
   - O segundo bloco, dentro de `@media (prefers-color-scheme: dark)`, são as cores do modo escuro.
3. O nome que aparece no topo está no trecho `Estudos da Ingryd` (procure com Ctrl+F). O nome da aba do navegador está em `<title>`.
4. Clique em **Commit changes**.

Se algo quebrar, o GitHub guarda todas as versões: em **History** dá para voltar a qualquer uma.

## Limites do plano gratuito do Supabase

- 1 GB para arquivos e 50 MB por arquivo.
- O projeto pausa após 1 semana sem uso. Basta entrar no painel do Supabase e clicar em **Restore**; nada é perdido.
