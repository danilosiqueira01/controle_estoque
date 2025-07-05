# controle_estoque
Controle de Estoque é uma webapp responsiva para gerenciar inventário em tempo real. Com visualização em grade ou lista, filtros por categoria, busca, estatísticas (total, valor, itens críticos) e webhooks para alertas de estoque baixo e relatórios via n8n. Conectado ao Supabase.

Visão Geral
Interface Clean e Mobile-First
Construída com HTML5, Tailwind CSS e módulo de fontes Inter, a UI se adapta perfeitamente a qualquer dispositivo, do desktop ao smartphone, oferecendo visualização em grade ou lista, além de filtros rápidos por categoria, busca por nome e botões de destaque (“Top 3 maior estoque”, “Estoque Baixo”, “Esgotado” etc.).

Persistência e Realtime com Supabase
Utiliza o Supabase (PostgreSQL + canais Realtime) para CRUD de produtos, atualização instantânea de listas e estatísticas sempre atualizadas (total de itens, valor total em estoque e quantidade em estoque baixo).

Alertas e Webhooks Automatizados

Ao cadastrar ou editar um produto que fique abaixo do estoque mínimo, dispara automaticamente um webhook para um fluxo n8n, permitindo enviar e-mails, SMS ou postar em canais de chat.

Botão “Enviar Relatório” dispara um webhook de relatório completo para seu workflow de automação, gerando planilhas ou sumários por e-mail.

Principais Funcionalidades
Dashboard Estatístico

Total de produtos cadastrados

Quantidade de itens com estoque abaixo do mínimo

Valor monetário total em estoque

Listagem Dinâmica

Visualização em grid ou lista, com indicadores coloridos (verde, amarelo, vermelho) que sinalizam o status de cada item

Responsivo: adapta colunas e botões em telas menores

Filtros e Busca

Busca em tempo real por nome ou categoria

Filtros rápidos: “Top 3 maior estoque”, “Top 3 menor estoque”, “Estoque Baixo”, “Esgotado”

Limpar filtros com um clique

Cadastro e Edição de Produtos

Formulário completo com validação: nome, categoria, quantidade, preço unitário e estoque mínimo

Feedback visual (pop-ups de sucesso/erro) e reset automático do formulário após operações

Exclusão Segura

Confirmação via confirm() antes de remover registros

Atualização imediata da interface e das estatísticas

Automação Realtime

Canal de Realtime do Supabase monitora todas as alterações na tabela de produtos e atualiza a lista para todos os usuários conectados

Tecnologias Utilizadas
Front-end: HTML5, Tailwind CSS, JavaScript (ES6+)

Back-end sem servidor: Supabase (PostgreSQL, Realtime, API REST/JS)

Automação de Workflows: n8n via webhooks

Hospedagem Estática: GitHub Pages, Vercel ou Netlify

Ícones: Heroicons SVG embutidos

Fonte: Google Fonts – Inter

