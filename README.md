# controle_estoque
Controle de Estoque é uma webapp responsiva para gerenciar inventário em tempo real. Com visualização em grade ou lista, filtros por categoria, busca, estatísticas (total, valor, itens críticos) e webhooks para alertas de estoque baixo e relatórios via n8n. Conectado ao Supabase.

## Descrição do Projeto

**Controle de Estoque – Ynayê** é uma aplicação web leve e responsiva, desenvolvida para pequenas e médias empresas que precisam gerenciar seu inventário de forma simples, visual e em tempo real. Ela combina uma interface intuitiva com funcionalidades avançadas de filtragem, relatórios automáticos e notificações de estoque baixo, garantindo que você tenha sempre o controle sobre seus produtos.

---

## Visão Geral

- **Interface clean e mobile-first**: construída com HTML5, Tailwind CSS e fonte Inter, adapta-se a qualquer dispositivo com visualização em grade ou lista.  
- **Supabase**: CRUD de produtos e sincronização em tempo real (Realtime).  
- **Alertas automáticos**: webhooks para notificações de estoque baixo e geração de relatórios via n8n.  
- **Filtros e busca**: categoria, Top 3 maior/menor estoque, estoque baixo, esgotado e busca instantânea por nome.

---

## Principais Funcionalidades

1. **Dashboard Estatístico**  
   - Total de produtos cadastrados  
   - Quantidade de itens com estoque abaixo do mínimo  
   - Valor monetário total em estoque  

2. **Listagem Dinâmica**  
   - Indicadores coloridos (verde, amarelo, vermelho) para status de cada item  
   - Responsivo: ajusta colunas e botões em telas menores  

3. **Filtros e Busca**  
   - Busca em tempo real por nome ou categoria  
   - Botões rápidos: Top 3 maior/menor, estoque baixo, esgotado  
   - Limpar filtros com um clique  

4. **Cadastro e Edição de Produtos**  
   - Formulário com validação: nome, categoria, quantidade, preço e estoque mínimo  
   - Feedback por pop-up e reset automático após salvar  

5. **Exclusão Segura**  
   - Confirmação via `confirm()` antes de remover  
   - Atualização imediata da interface e estatísticas  

6. **Automação Realtime**  
   - Canal Realtime do Supabase escuta mudanças na tabela e atualiza todos os usuários conectados  

---

## Tecnologias Utilizadas

- **Front-end**: HTML5, Tailwind CSS, JavaScript (ES6+)  
- **Back-end sem servidor**: Supabase (PostgreSQL, Realtime, API REST/JS)  
- **Automação de Workflows**: n8n via webhooks  
- **Hospedagem Estática**: GitHub Pages, Vercel ou Netlify  
- **Ícones**: Heroicons SVG embutidos  
- **Fonte**: Google Fonts – Inter  


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

