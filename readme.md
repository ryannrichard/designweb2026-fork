# Tarefa 33 — Meu Portfólio com DaisyUI

Fiz esta página pessoal para treinar o uso dos componentes do DaisyUI e organizar minhas habilidades e projetos.

## 1. Componentes DaisyUI que usei
* **Navbar**: No topo da página para criar o menu de navegação.
* **Hero**: Logo abaixo do menu para fazer a apresentação principal com meu nome e botões de chamada.
* **Badges**: Na seção "Sobre Mim" para destacar minhas tecnologias (HTML, Tailwind, DaisyUI, etc).
* **Cards**: Na seção de projetos, usando a estrutura com título, descrição e botão de ação.
* **Alert**: Um aviso de informação (`alert-info`) indicando minha disponibilidade para oportunidades.
* **Input**: Nos campos de nome e e-mail do formulário de contato.
* **Buttons (`btn`)**: Usei estilos variados como `btn-primary`, `btn-outline` e `btn-sm` para dar uma certa hierarquia pros botões.

## 2. Justificativa
Decidi combinar a **Navbar** com o **Hero** no cabeçalho porque a navbar mantém a navegação sempre acessível no topo, enquanto o hero traz um impacto visual logo de cara, apresentando quem eu sou e o que faço de forma direta.

## 3. Pontos de ajuste
O DaisyUI resolveu a parte visual dos componentes, mas usei classes do Tailwind para ajustar a estrutura e o espaçamento:
1. **Controle de largura no `<main>`**: Usei `max-w-6xl mx-auto px-4` para o conteúdo ficar centralizado e não esticar demais em monitores grandes.
2. **Grid dos projetos**: Usei `grid grid-cols-1 md:grid-cols-3 gap-6` para deixar os 3 cards organizados em colunas no computador e empilhados no celular.

## 4. Teste de Temas
Testei a página usando os temas **`emerald`** e **`dark`**. 
Preferi o **`emerald`**, pois as cores claras deixaram o portfólio com um visual mais agradável ao meu ver, fora que também ficou semelhante ao ifrn.