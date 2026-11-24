# Lexicon — O Prazer de Saber

Aplicativo web progressivo (PWA) particular, instalável na tela inicial do iPhone pelo Safari. Não é um app nativo SwiftUI e não exige App Store.

## O que já funciona
- 20 descobertas escritas e interligadas (palavras, mitologias, filosofia, literatura e civilizações).
- Descoberta aleatória e trilhas livres por assuntos relacionados.
- Pesquisa por título, tema e tags, filtros por categoria.
- Favoritos, notas pessoais e histórico de descobertas (armazenamento local no dispositivo).
- Pequeno desafio de associação, sem pontos nem metas.
- Leitura em voz alta via Web Speech API quando suportada.
- Exportação em JSON de favoritos e anotações.
- PWA com service worker e arquivos offline após primeiro acesso por HTTPS.

## Publicação em GitHub Pages (sem programação)
1. Crie um repositório **privado ou público**, de acordo com sua preferência. Atenção: GitHub Pages em contas e planos comuns pode exigir que o repositório seja público; um repositório público expõe o código e o conteúdo editorial, **não** as suas notas locais.
2. Envie **todos os arquivos desta pasta** para a raiz do repositório: index.html, app.js, data.js, style.css, manifest.webmanifest, sw.js e os dois PNGs.
3. No GitHub, abra **Settings → Pages** e configure **Deploy from a branch**, branch `main`, pasta `/(root)`, caso seu plano/repositório permita Pages.
4. Abra a URL HTTPS apresentada pelo GitHub Pages no Safari do iPhone.
5. Toque em **Compartilhar → Adicionar à Tela de Início**. Confirme **Lexicon**.

**Privacidade:** o conteúdo padrão é público se hospedado em Pages público. Favoritos e notas ficam no `localStorage` do navegador deste dispositivo, não são enviados ao GitHub. Limpar os dados do Safari, trocar de dispositivo ou desinstalar pode apagar essas informações. Use **Coleção → Exportar** para fazer backup. Se precisar acesso realmente restrito por autenticação, será necessário adicionar uma camada de autenticação e hospedagem apropriada; não chame o endereço público de privado.

## Teste local
Use `python -m http.server 8000` na pasta e acesse `http://localhost:8000` (desktop). Para testar offline e a instalação no iPhone, publique via HTTPS.

## Limites da versão
Não tem IA nem pesquisa web dinâmica, não sincroniza entre dispositivos, não envia notificações, e ainda não dispõe de um catálogo extenso. A reescrita de textos eruditos foi retirada da direção principal para privilegiar a exploração livre. A pronúncia depende de vozes disponíveis no navegador iOS. Fontes são referências de leitura, não verificação automatizada nem links bibliográficos completos.
