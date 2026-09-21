## Tarefa 10 – Seção de eventos

**Objetivo:** A partir do código HTML limpo (sem classes), você deve adicionar classes Tailwind para estilizar a seção "Eventos" do site do IFRN, reproduzindo o layout da imagem de referência.


### regras

- Use apenas classes utilitárias do Tailwind – sem CSS customizado.
- Não modifique a estrutura HTML (tags, conteúdo, atributos href, src, etc.).
- Consulte o Cheatsheet para encontrar as classes adequadas.


---

## Passo a passo para execução

1. **Atualize seu fork** do repositório da turma.
2. **Crie uma nova branch** para esta tarefa:  
   ```bash
   git checkout -b features/atividade-10-evento
   ```
3. **Insira classes Tailwind** em cada elemento para reconstruir o layout, visualizando como está o site do IFRN e criar a estrutura adequada com as classes mais proeminentes.
   
4. **Commit e push**:
   ```bash
   git add .
   git commit -m "Atividade 10 - Seção de eventos"
   git push origin atividade-9-footer
   ```

### Passo 4 – Enviar o link no Google Sala de Aula
- No GitHub, vá até seu repositório fork.
- No seletor de branches, escolha atividade-1.
- Copie a URL (ex: https://github.com/SEU_USUARIO/turma-design-web/tree/atividade-1).
- Cole esse link no campo de entrega da tarefa.


## 3ª Semana 

Fizemos algumas atividades, focados no Github. Criamos e clonamos nosso repositório principal.

### Passo 1 – Fork do repositório

- Acesse: https://github.com/professor/turma-design-web
- Clique no botão Fork (canto superior direito). Isso criará uma cópia na sua conta. 

### Passo 2 – Clonar o fork
Abra o terminal (Git Bash, PowerShell ou terminal integrado do VS Code) e execute

```
git clone https://github.com/SEU_USUARIO/turma-design-web.git
cd turma-design-web
```



Arquivo de codigo compartilhado

## 2ª Semana 

### Cartão de Apresentação – Bruno Nakamura

Projeto didático para ensinar a integração entre **HTML semântico** e **SCSS** (pré-processador CSS).

## Estrutura

projeto/

├── index.html 

├── scss/

└── style.scss 

└── css/

└── style.css # Arquivo gerado pelo SCSS (não edite jamais ou vai perder tudo para sempre)


## Como usar

1. **Clone ou baixe** os arquivos.
2. **Compile o SCSS** para CSS:
   - Com o Sass instalado: `sass scss/style.scss css/style.css --watch`
   - Ou use a extensão "Live Sass Compiler" no VS Code.
3. **Abra** o `index.html` no navegador.

## Personalize

- **Cores**: altere as variáveis no início do `style.scss` (`$color-primary`, `$color-secondary`, etc.).
- **Imagem**: substitua a URL placeholder (`https://via.placeholder.com/...`) pelo seu próprio avatar.
- **Conteúdo**: edite o HTML para mudar texto, tecnologias e links.

## Boas práticas aplicadas

- Tags HTML semânticas (`header`, `main`, `section`, `footer`)
- Atributos de acessibilidade (`role`, `aria-label`, `focus-visible`)
- Responsividade com mixins (mobile-first)
- Código SCSS organizado com variáveis e aninhamento
