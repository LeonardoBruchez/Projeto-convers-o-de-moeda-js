<<<<<<< HEAD
# 💱 Conversor de Moedas

Um projeto simples e elegante para conversão de moedas estrangeiras para Real Brasileiro, desenvolvido durante a trilha Fullstack da Rocketseat com foco no aprendizado de JavaScript.

## 📋 Sobre o Projeto

Este projeto foi criado com o objetivo de praticar e consolidar conhecimentos em JavaScript, utilizando HTML e CSS já prontos. O conversor permite transformar valores em Dólar Americano (USD), Euro (EUR) e Libra Esterlina (GBP) para Real Brasileiro (BRL).

## ✨ Funcionalidades

- **Conversão de Moedas**: Converta USD, EUR e GBP para BRL
- **Validação de Input**: Aceita apenas números no campo de valor
- **Interface Responsiva**: Design moderno e intuitivo
- **Formatação Automática**: Valores exibidos no padrão brasileiro (R$ 0,00)
- **Cotação em Tempo Real**: Exibe a cotação da moeda selecionada

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica do projeto
- **CSS3**: Estilização e layout responsivo
- **JavaScript Vanilla**: Lógica de conversão e manipulação do DOM
- **Google Fonts**: Tipografia (Inter e IBM Plex Mono)

## 📁 Estrutura do Projeto

```
Projeto conversão de moeda Java Script/
├── img/
│   ├── bg.png          # Imagem de fundo
│   ├── check.svg       # Ícone de check
│   ├── chevron-down.svg # Ícone do dropdown
│   └── logo.svg        # Logo do projeto
├── index.html          # Página principal
├── scripts.js          # Lógica JavaScript
├── styles.css          # Estilos CSS
└── README.md           # Documentação
```

## 🚀 Como Executar

1. Clone ou baixe o projeto
2. Abra o arquivo `index.html` em qualquer navegador moderno
3. Digite um valor no campo "valor"
4. Selecione a moeda desejada
5. Clique em "Converter em reais"
6. Veja o resultado da conversão!

## 💡 Principais Conceitos JavaScript Aplicados

### 1. **Manipulação do DOM**
```javascript
const form = document.querySelector("form")
const amount = document.getElementById("amount")
const currency = document.getElementById("currency")
```

### 2. **Event Listeners**
```javascript
amount.addEventListener("input", () => {
  const hasCharactersRegex = /\D+/g
  amount.value = amount.value.replace(hasCharactersRegex, "")
})
```

### 3. **Prevenção de Comportamento Padrão**
```javascript
form.onsubmit = (event) => {
  event.preventDefault()
  // ... lógica de conversão
}
```

### 4. **Estruturas de Controle (Switch)**
```javascript
switch(currency.value){
  case "USD":
    convertCurrency(amount.value, USD, "US$")
    break
  case "EUR":
    convertCurrency(amount.value, EUR, "€")
    break
  case "GBP":
    convertCurrency(amount.value, GBP, "£")
    break
}
```

### 5. **Tratamento de Erros**
```javascript
try {
  // ... lógica principal
} catch (error) {
  console.log(error)
  alert("Não foi possível converter. Tente novamente mais tarde.")
}
```

### 6. **Formatação de Moeda**
```javascript
function formatCurrencyBRL(value){
  return Number(value).toLocaleString("pt-BR", {
    style: "currency",
    currency: "BRL",
  })
}
```

### 7. **Manipulação de Classes CSS**
```javascript
footer.classList.add("show-result")
footer.classList.remove("show-result")
```

### 8. **Validação de Dados**
```javascript
if(isNaN(total)){
  return alert("Por favor,digite o valor corretamente para converter.")
}
```

## 📊 Cotações Utilizadas

- **USD**: R$ 5,28
- **EUR**: R$ 6,24
- **GBP**: R$ 7,14

*Nota: As cotações são fixas no código. Em um projeto real, seria ideal consumir uma API de cotações em tempo real.*

## 🎨 Design

O projeto apresenta um design moderno com:
- **Paleta de cores**: Tons de azul e roxo (#1f2151, #2f3279, #4a5dcd)
- **Tipografia**: Inter para textos e IBM Plex Mono para valores
- **Layout**: Centralizado com formulário em card
- **Responsividade**: Adaptável a diferentes tamanhos de tela

## 📚 Objetivos de Aprendizado

Este projeto foi desenvolvido para praticar:

- ✅ Manipulação do DOM
- ✅ Event Listeners
- ✅ Validação de formulários
- ✅ Formatação de dados
- ✅ Tratamento de erros
- ✅ Estruturas de controle
- ✅ Funções e modularização
- ✅ CSS Classes dinâmicas

## 🔮 Possíveis Melhorias

- Integração com API de cotações em tempo real
- Histórico de conversões
- Mais moedas disponíveis
- Gráficos de variação das cotações
- Armazenamento local das conversões
- Modo escuro/claro

## 📝 Licença

Este projeto foi desenvolvido para fins educacionais durante a trilha Fullstack da Rocketseat.

---

**Desenvolvido com 💜 durante a trilha Fullstack da Rocketseat**
=======
# Projeto-convers-o-de-moeda-js
Este projeto é um conversor de moedas em JavaScript. A aplicação permite converter valores entre moedas, validar a entrada de dados para aceitar apenas números e selecionar diferentes moedas. É uma ótima adição ao portfólio, demonstrando habilidades em manipulação do DOM e lógica de programação.
>>>>>>> 369b6ae1c8a0917058513511289a4752ebf26f2b
