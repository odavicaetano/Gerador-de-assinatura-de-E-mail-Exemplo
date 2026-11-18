# Gerador de assinatura de E-mail | Exemplo (PWA)

Esta edição preserva a aparência azul e todas as funcionalidades da versão HTML original.

## Publicar

1. Publique **todos os arquivos** desta pasta juntos na raiz do site (ou de um repositório do GitHub Pages).
2. Acesse o endereço publicado em HTTPS. Service Workers não funcionam ao abrir o arquivo diretamente via `file://`.
3. Entre uma vez com internet e aguarde a instalação do Service Worker. Depois, feche e abra novamente sem conexão para validar.
4. No Chrome/Edge, use a opção de instalar o aplicativo. No Safari no iOS, abra Compartilhar > Adicionar à Tela de Início.

## Atualizar o site

O Service Worker usa Cache First para abertura instantânea. Ao editar `index.html`, altere a versão de `CACHE_NAME` em `sw.js` (por exemplo, `v1` para `v2`) para atualizar o conteúdo cacheado. Recarregue o site online e reinicie o aplicativo instalado.

## Privacidade e offline

Não existe armazenamento de formulário, dados pessoais nem preferências. O cache mantém apenas os arquivos públicos da aplicação. CSS e JavaScript estão incorporados ao HTML, os gráficos são vetoriais locais e a fonte é Arial do sistema. Não há dependências de CDN ou fontes remotas nesta versão.

## Arquivos

- `index.html`: app original com integração PWA
- `manifest.json`: informações de instalação
- `sw.js`: cache de arquivos estáticos e fallback de navegação
- `icon.svg`, `icon-192.png`, `icon-512.png`: ícones baseados no favicon original
