# Sistema de Vendas — Modelo Demonstrativo

## Objetivo
Este projeto é um protótipo de apresentação de um sistema de vendas para produtos agrícolas. Ele preserva a interface e os fluxos de demonstração sem depender de serviços externos.

## Arquitetura
- `index.html`: estrutura da aplicação e adaptador local de demonstração.
- `css/style.css`: estilos e layout responsivo.
- `js/script.js`: regras de negócio, cálculos, renderização, vendas, estoque, gastos e relatórios.
- `assets/`, `icons/`, `img/`: recursos visuais e ícones.
- `sw.js`: cache para uso como aplicação web instalável em hospedagem HTTPS.

## Sem autenticação e sem banco de dados
Não há Firebase, Firestore, autenticação, API de vendas ou banco de dados. O sistema abre diretamente no painel. O adaptador em `index.html` fornece dados fictícios e operações em memória para permitir demonstrar cadastros, edições, cancelamentos, estoque e gastos.

## Persistência
Os dados são mantidos somente na memória da aba atual. Ao atualizar ou fechar a página, o conjunto inicial de demonstração é carregado novamente. Nenhuma venda real deve ser registrada nesta versão.

## Como executar
Abra `index.html` em um navegador moderno. Para testar recursos de PWA/service worker, publique os arquivos em hospedagem estática HTTPS.

## Tecnologias
HTML5, CSS3 e JavaScript puro. Bibliotecas externas opcionais usadas pela interface incluem Lucide, jsPDF e Google Fonts.
