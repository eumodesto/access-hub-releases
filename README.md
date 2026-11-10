# Access Hub

**Use Claude Code, Cursor, Codex e OpenCode no mesmo projeto, troque de uma IA para outra a
qualquer hora e nunca mais copie token para `.env`.**

O Access Hub é a central de quem desenvolve com IA no Windows: cofre de chaves por projeto,
IDEs abertas já conectadas à pasta, scan de segurança e as senhas dos painéis dos clientes,
tudo criptografado no seu computador.

**[⬇ Baixar a versão mais nova para Windows](https://github.com/eumodesto/access-hub-releases/releases/latest)**
· Instalador sem pedir administrador · Atualiza sozinho · Em português

> Este repositório guarda só os instaladores e as atualizações. O código-fonte não fica
> aqui.

---

## O que ele resolve

- O crédito de uma IA acabou no meio da tarefa? Abra outra IDE e continue: as chaves já
  estão lá, sem configurar nada de novo.
- Tokens espalhados em `.env`, bloco de notas e conversas passam a morar num cofre só.
- Uma sessão da IA nunca pega a chave de outro cliente por engano.
- Segredos não vazam para o GitHub nem para o site publicado sem você saber.

## Principais recursos

### IDEs conectadas com um clique

- **Abrir nova sessão** no Claude Code, no Cursor, no Codex ou no OpenCode, já na pasta do
  projeto. O app mostra só as IDEs instaladas no computador.
- **Servidor MCP do Access Hub** registrado na pasta: a IA consulta o projeto, os deploys
  da Vercel e o relatório de segurança sem nunca receber o token.
- **Nota de passagem**: a sessão que estava trabalhando registra onde parou, e a próxima,
  até em outra IDE, lê ao começar.
- **`access-hub run -- <comando>`**: roda o servidor de desenvolvimento, scripts e testes
  com as chaves e as variáveis do app entregues na hora, sem gravar nada em disco.
- **Git sem senha e sem token na URL**, pelo credential helper do Access Hub.

### Cofre de chaves por projeto

- GitHub, Vercel, Supabase, Resend, OpenAI, OpenRouter, Mercado Pago e PagBank.
- **A IA usa a chave, mas não vê a chave.** Ela é entregue ao Git, ao terminal e às
  ferramentas só no momento do uso.
- Cada chave fica presa ao projeto e ao ambiente dela, e limitada ao que você liberou: os
  repositórios, os projetos da Vercel, os projetos do Supabase ou os domínios do Resend que
  você marcou.
- Ao guardar, o app testa a chave e lista o que ela alcança. O sino avisa quando uma chave
  para de funcionar.
- Mercado Pago completo para o Checkout Transparente: Access Token, Public Key e a
  assinatura secreta dos Webhooks.

### Um token, e o app resolve o resto

- Ao conectar um projeto, o Access Hub lê o código e mostra quais chaves estão faltando,
  com o passo a passo e o link direto para gerar cada uma.
- Projeto novo? O app cria o repositório no GitHub, prepara a pasta e conecta tudo.
- As variáveis do app (Supabase, Vercel) são buscadas a cada execução e conferidas entre os
  serviços, com **Desfazer** em cada mudança.
- Quando algo dá errado, o aviso diz o motivo e leva à página certa para corrigir.

### Scan de segurança

- Procura segredos no histórico do Git (todos os branches), nos arquivos, nos `.env` e no
  site publicado.
- Compara com o valor real das suas chaves e com os formatos conhecidos de GitHub, OpenAI,
  Anthropic, Stripe, Supabase, AWS, Mercado Pago, chaves privadas e outros.
- Trava antes do commit: barra segredo e `.env` antes de sair do seu computador.
- **Copiar relatório para a IDE**: junta os achados num texto pronto para a IA corrigir, sem
  levar o valor de nenhuma chave.

### Clientes, projetos e senhas dos painéis

- Tudo organizado por cliente e projeto, com ambientes separados (Desenvolvimento,
  Produção…).
- Cadastro de projeto em 4 passos guiados.
- Login de cada painel do cliente (Vercel, Supabase, Google, hospedagem…) guardado por
  cliente, com códigos de recuperação e anotações. Copiar a senha limpa a área de
  transferência em 30 segundos.
- Essas senhas nunca vão para a IA, para o MCP nem para o Git.

### Seus dados, no seu computador

- Criptografia AES-256-GCM, com uma chave própria para cada segredo.
- O cofre abre pelo seu usuário do Windows, sem senha mestra para lembrar todo dia.
- O app só aceita conexões da própria máquina, e nenhuma tela devolve o segredo depois de
  guardado.
- Cada entrega de chave, recusa, cópia de senha, exportação e importação fica registrada,
  sem gravar o valor.
- **Exporte o cofre inteiro** num arquivo protegido por senha e importe em outro computador.
  Há cópia automática diária, e desinstalar o app não apaga o cofre.

## Em breve

- **Biblioteca**: componentes com prévia ao vivo e **Skills** para a IA (a primeira é o
  HyperFrames), que entram no projeto com um clique e se atualizam sozinhas.
- Conta, teste grátis e assinatura por Pix ou cartão.

## Instalação

1. Baixe o `Access-Hub-Setup-X.Y.Z.exe` na
   [versão mais nova](https://github.com/eumodesto/access-hub-releases/releases/latest).
2. Abra o instalador. Ele instala só para o seu usuário, sem pedir administrador.
3. O instalador ainda não tem assinatura digital, por isso o Windows pode mostrar o aviso
   do SmartScreen na primeira vez. Clique em **Mais informações → Executar assim mesmo**.
4. Na primeira abertura, crie o cofre e cadastre o primeiro projeto.

**Requisitos:** Windows 10 ou 11 (64 bits). Para abrir sessões pelo app, tenha instalado o
Claude, o Cursor, o Codex ou o OpenCode.

## Atualizações

O app confere se há versão nova ao abrir e a cada 6 horas, baixa em segundo plano e instala
quando você reinicia (pelo sino, pela bandeja ou em Configurações → Aplicativo). O que muda
em cada versão está nas [notas das versões](https://github.com/eumodesto/access-hub-releases/releases).

---

Access Hub · IA para Todos
