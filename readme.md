=======
# Repositório da turma de Design Web 2026
=======
# Calculadora Vue.js — Aula 01

Atividade prática da primeira aula de Vue.js.
## Objetivo

Construir uma calculadora com as **quatro operações** (`+`, `−`, `×`, `÷`) usando **apenas Vue.js** via CDN.

**Toda a estrutura visual e html com Vue já estão prontos.** Você só precisa implementar ** os 3 métodos** que fazem a funcionalidade da calculadora.
>>>>>>> upstream/main


**Já está pronto:**

- Todo o HTML (a `<div id="app">`, os botões, o visor)
- Todo o visual em Tailwind CSS + DaisyUI
- Os botões já estão conectados aos métodos via `@click`
- A estrutura `Vue.createApp({...}).mount('#app')`
- O `data()` com os 4 campos do estado
- O método `clear()` completo como exemplo

**Falta fazer:**

3 métodos dentro do `<script>`:

| TODO | Método | Funcionalidade |
|---|---|---|
| **TODO 1** | `appendDigit(digit)` | Digita um número no visor |
| **TODO 2** | `setOperator(op)` | Registra o operador pendente |
| **TODO 3** | `calculate()` | Executa a conta |

Abra o `index.html` e siga os comentários `TODO` em cada método.

### TODO 1 — `appendDigit(digit)`

Recebe um dígito (`'0'` a `'9'`) e atualiza o visor.

**Regras:**
1. Se `waitingForSecond` for `true`: **substitui** `this.display` pelo dígito e marca `waitingForSecond = false`.
2. Senão, se `this.display === '0'`: **substitui** pelo dígito (para nao concatenar).
3. Senão: **concatena** — `this.display = this.display + digit`.

**Exemplos:**
- `display='0'`, `digit='5'` → `display='5'`
- `display='12'`, `digit='3'` → `display='123'`
- `display='12'`, `waitingForSecond=true`, `digit='7'` → `display='7'`

### TODO 2 — `setOperator(op)`

Recebe um operador (`'+'`, `'-'`, `'*'`, `'/'`) e o registra para a próxima conta.

**Regras:**
1. Se `this.display === 'Erro'`: **saia** (`return`) sem fazer nada.
2. Se `this.operator !== null` **e** `this.waitingForSecond === false`: chame `this.calculate()` primeiro (para encadear `5 + 3 ×`).
3. `this.firstOperand = parseFloat(this.display)`
4. `this.operator = op`
5. `this.waitingForSecond = true`

### TODO 3 — `calculate()`

Executa a operação pendente e mostra o resultado.

**Regras:**
1. Se `this.operator === null` **ou** `this.firstOperand === null`: **retorne** (nada a fazer).
2. `const a = this.firstOperand`
3. `const b = parseFloat(this.display)`
4. Aplique o operador:
   - `'+'` → `a + b`
   - `'-'` → `a - b`
   - `'*'` → `a * b`
   - `'/'` → se `b === 0` → `'Erro'`; senão `a / b`
5. `this.display = String(resultado)`
6. `this.firstOperand = null`
7. `this.operator = null`
8. `this.waitingForSecond = true`

### Referência: o `clear()` já está pronto

Use como exemplo de como acessar o estado com `this`:

```js
clear() {
  this.display = '0';
  this.firstOperand = null;
  this.operator = null;
  this.waitingForSecond = false;
}
```

## Como testar

| Cliques | Visor deve mostrar |
|---|---|
| `7` `+` `5` `=` | `12` |
| `9` `×` `8` `=` | `72` |
| `1` `0` `÷` `4` `=` | `2.5` |
| `8` `−` `3` `=` | `5` |
| `5` `÷` `0` `=` | `Erro` |
| `7` `+` `3` `=` `×` `2` `=` | `20` |
| `7` `+` `3` `×` `2` `=` | `20` |
| `C` | `0` |
| `5` `÷` `0` `=` `7` `+` `1` `=` | `8` (recupera do `Erro`) |



## Entrega no GSA

```bash
git checkout -b aula-01-calculadora
git add .
git commit -m "Aula 01 — Calculadora Vue"
git push -u origin aula-01-calculadora
```

<<<<<<< HEAD
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
>>>>>>> upstream/main
=======
No GitHub, abra a aba **Branches**, encontre `aula-01-calculadora` e **copie a URL** da branch (algo como `https://github.com/<usuario>/<repo>/tree/aula-01-calculadora`). Cole esse link no GSA.
>>>>>>> upstream/main
