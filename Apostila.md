# 📌 React e React Native

Se você já ouviu falar de **React** e **React Native**, mas não entende exatamente o que são ou como funcionam, esta explicação vai te ajudar a entender tudo de forma simples. Vamos lá! 🚀  

---

## 🔹 O Que é o React?  

**React** é uma **biblioteca** JavaScript criada pelo **Facebook** (agora Meta) para facilitar a construção de **interfaces de usuário interativas** em aplicações web.  

### 📌 Por que o React foi criado?  
Antes do React, os sites eram criados com **HTML, CSS e JavaScript puro**, o que dificultava a manutenção e atualização da interface. Com o React, ficou muito mais fácil construir páginas dinâmicas e interativas.  

### 📌 Como o React Funciona?  
O React usa um conceito chamado **Componentes**. Um **componente** é como um “bloco de LEGO” reutilizável que pode ser combinado para criar interfaces complexas.  

Exemplo de um componente React que exibe um botão:  

```jsx
function Botao() {
  return <button>Clique aqui</button>;
}
```

Isso significa que você pode **reutilizar** esse botão em várias partes do seu site, sem precisar reescrever o código toda vez.  

### 📌 O Que Torna o React Especial?  
✅ **Reutilização de Componentes** → Escreva um botão uma vez e use várias vezes!  
✅ **Atualização Inteligente** → Quando algo muda na página, o React **atualiza só o que precisa**, sem recarregar tudo.  
✅ **Facilidade de Aprendizado** → Se você conhece JavaScript, pode aprender React rapidamente.  

Agora que entendemos o React, vamos falar do **React Native**!  

---

## 🔹 O Que é o React Native?  

**React Native** é um **framework** baseado no React, mas criado para desenvolver **aplicativos móveis** para **Android e iOS**.  

### 📌 Qual a Diferença Entre React e React Native?  
| Característica       | React (Web)           | React Native (Mobile) |
|----------------------|----------------------|----------------------|
| Onde é usado?       | Sites e Web Apps      | Apps para Android e iOS |
| Linguagem Principal | JavaScript e JSX      | JavaScript e JSX |
| Componentes Padrão  | `<div>`, `<button>`   | `<View>`, `<Text>` |

### 📌 Como o React Native Funciona?  
Assim como o React cria interfaces para sites, o **React Native cria telas para aplicativos**. Mas, em vez de usar elementos HTML (`<div>`, `<button>`), ele usa componentes móveis como:  

✅ **`<View>`** → Funciona como uma `<div>` no React Web, usado para agrupar elementos.  
✅ **`<Text>`** → Substitui o `<p>` ou `<h1>`, pois não existe HTML em aplicativos nativos.  
✅ **`<Button>`** → Cria botões nativos para Android e iOS.  

Exemplo de um componente React Native que exibe um botão:

```jsx
import { View, Text, Button } from 'react-native';

function MeuApp() {
  return (
    <View>
      <Text>Olá, Mundo!</Text>
      <Button title="Clique aqui" onPress={() => alert("Botão clicado!")} />
    </View>
  );
}
```

### 📌 Principais Vantagens do React Native  
✅ **Código Único para Android e iOS** → Escreva uma vez e use nos dois sistemas!  
✅ **Rápido e Eficiente** → Usa componentes nativos para melhor desempenho.  
✅ **Facilidade de Aprendizado** → Se você já conhece React, aprender React Native é muito mais fácil.  

---



| Tecnologia    | Para quê serve?            | Onde é usado?      |
|--------------|---------------------------|--------------------|
| **React**    | Criar interfaces web       | Navegadores       |
| **React Native** | Criar apps para celular | Android e iOS |

Se você quer criar **sites interativos**, aprenda **React**.  
Se quer criar **aplicativos móveis**, aprenda **React Native**.  

💡 **E o melhor? Você pode aprender os dois e se tornar um desenvolvedor Full Stack!** 🚀



# 📌 O Que é o **Expo Framework**? 

Se você já ouviu falar de **React Native**, provavelmente também já viu o nome **Expo** por aí. Mas o que é **Expo**? Para que ele serve? E por que ele facilita tanto o desenvolvimento de aplicativos móveis? 🤔  

Vamos entender tudo isso de forma simples! 🚀  

---

## 🔹 O Que é o **Expo**?  

O **Expo** é um **framework** e uma **plataforma** que facilita a criação de aplicativos móveis usando **React Native**. Ele fornece ferramentas que tornam o processo de desenvolvimento mais rápido e acessível, **sem precisar configurar tudo manualmente**.  

> 📌 **Simplificando:** O Expo é como um "atalho" que ajuda você a criar apps React Native sem precisar se preocupar com configurações complicadas.  

---

## 🔹 Por Que o Expo Foi Criado?  

Desenvolver aplicativos nativos pode ser **complicado**. Normalmente, para rodar um app React Native no celular, você precisaria:  

✅ Instalar e configurar o **Android Studio** (para Android) e o **Xcode** (para iOS).  
✅ Baixar e configurar emuladores de Android e iOS.  
✅ Configurar o **React Native CLI**, que exige mais ajustes técnicos.  

Com o **Expo**, você pula essa parte! Ele fornece um **ambiente pronto** para começar a desenvolver imediatamente.  

---

## 🔹 Como o Expo Facilita o Desenvolvimento?  

O Expo oferece diversas facilidades, como:  

### ✅ 1. **Testar o App Sem Emulador**  
Com o **Expo Go** (um aplicativo gratuito para Android e iOS), você pode testar seu app diretamente no seu celular **escaneando um QR Code**.  

**Sem Expo:** Você precisa de um computador potente e configurar um emulador.  
**Com Expo:** Você só instala o Expo Go no celular e testa o app em segundos!  

### ✅ 2. **Instalação Fácil**  
Criar um novo projeto com React Native tradicionalmente envolve várias configurações manuais. Com o Expo, basta um único comando:  

```bash
npx create-expo-app MeuApp
```

E pronto! Você já tem um projeto configurado. 🎉  

### ✅ 3. **Bibliotecas e Recursos Prontos**  
O Expo já vem com várias funcionalidades que seriam difíceis de configurar sozinho, como:  

📸 **Acesso à Câmera**  
📍 **GPS e Localização**  
📤 **Compartilhamento de Arquivos**  
🔔 **Notificações Push**  

Para usar essas funções, basta instalar pacotes prontos do Expo, como:  

```bash
npx expo install expo-camera
```

E depois usar no código:  

```jsx
import { Camera } from 'expo-camera';
```

Muito mais fácil, né?  

---

## 🔹 Como o Expo Funciona?  

O Expo é dividido em **três partes principais**:  

### 📌 1. **Expo CLI** (Interface de Linha de Comando)  
É a ferramenta usada para criar e rodar projetos Expo. Você usa comandos simples no terminal, como:  

```bash
npx expo start
```

Isso abre um painel interativo com um **QR Code** para testar o app no celular.  

### 📌 2. **Expo Go** (App para Testes)  
Um aplicativo gratuito disponível na Play Store e App Store. Com ele, você pode rodar seu app no celular **sem precisar conectar cabos ou instalar emuladores**.  

### 📌 3. **Expo SDK** (Conjunto de Bibliotecas)  
São bibliotecas prontas para usar funcionalidades como câmera, GPS, notificações, etc., sem precisar de configurações extras.  

---

## 🔹 Expo vs React Native CLI  

O **React Native** pode ser usado de duas formas:  

| Característica        | **Expo** 🏆 (Mais fácil) | **React Native CLI** (Mais flexível) |
|----------------------|----------------------|----------------------|
| Configuração        | Super rápida ✅      | Complexa ❌          |
| Emulador necessário? | Não, só usar o Expo Go ✅ | Sim, precisa de Android Studio ❌ |
| Acesso a código nativo (Android/iOS) | Não ❌ | Sim ✅ |
| Facilidade de atualização | Sim, atualizações automáticas ✅ | Manual, pode quebrar o projeto ❌ |

**Quando usar Expo?**  
✅ Se você está começando com React Native.  
✅ Se quer testar rapidamente um app no celular.  
✅ Se precisa de um app simples e rápido.  

**Quando NÃO usar Expo?**  
❌ Se você precisa modificar código nativo (Android/iOS).  
❌ Se precisa adicionar pacotes que o Expo não suporta.  

> 💡 **Dica:** Você pode começar com Expo e depois migrar para React Native CLI se precisar de mais controle.  

---


✅ **Expo facilita o desenvolvimento de aplicativos com React Native.**  
✅ **Não precisa instalar emuladores ou configurar código nativo.**  
✅ **Vem com várias funcionalidades prontas, como câmera e GPS.**  
✅ **Perfeito para iniciantes e prototipagem rápida!** 🚀  

Se você quer criar um app mobile **sem complicação**, o **Expo é a melhor opção!** 🎉

### O que é o DOM (Document Object Model) no contexto de navegadores com JavaScript?

O **DOM (Document Object Model)** é uma interface de programação que representa a estrutura de um documento HTML ou XML como uma árvore de objetos. Ele permite que linguagens de programação, como o **JavaScript**, interajam dinamicamente com o conteúdo, estrutura e estilo da página web.

---

## 🔹 Como o DOM funciona?

Quando um navegador carrega uma página web, ele interpreta o código HTML e constrói um modelo estruturado do documento na memória. Esse modelo é o **DOM**, que organiza os elementos da página em uma hierarquia de nós.

Por exemplo, o seguinte código HTML:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Exemplo DOM</title>
</head>
<body>
    <h1 id="titulo">Olá, Mundo!</h1>
    <p class="descricao">Esse é um exemplo de manipulação do DOM.</p>
</body>
</html>
```

É transformado em uma árvore DOM assim:

```
Document
│
├── html
│   ├── head
│   │   ├── title ("Exemplo DOM")
│   ├── body
│       ├── h1 (id="titulo") ("Olá, Mundo!")
│       ├── p (class="descricao") ("Esse é um exemplo de manipulação do DOM.")
```

Essa estrutura permite que o JavaScript acesse e manipule os elementos da página de forma dinâmica.

---

## 🔹 Principais Componentes do DOM

### 1️⃣ **Nós (Nodes)**
Cada parte do documento HTML é representada como um **nó** no DOM. Existem diferentes tipos de nós, como:
- **Elemento (Element Nodes)** – Representam tags HTML (`<h1>`, `<p>`, `<div>`, etc.).
- **Atributo (Attribute Nodes)** – Representam atributos dos elementos (`id`, `class`, `src`, etc.).
- **Texto (Text Nodes)** – Representam o conteúdo textual dentro dos elementos.
- **Comentário (Comment Nodes)** – Representam comentários `<!-- Isso é um comentário -->`.

### 2️⃣ **Árvore DOM**
A estrutura do DOM segue uma hierarquia em forma de árvore:
- O nó raiz é o **document** (representando o documento HTML inteiro).
- Dentro dele, temos **elementos filhos** (`<html>`, `<head>`, `<body>`, etc.).
- Cada elemento pode ter **outros elementos filhos**, atributos e nós de texto.

### 3️⃣ **Objeto `document`**
O objeto `document` é a principal interface do DOM em JavaScript e permite acessar elementos da página.

Exemplo de acesso ao título da página:
```javascript
console.log(document.title); // "Exemplo DOM"
```

---

## 🔹 Manipulação do DOM com JavaScript

### 🔸 **Selecionando Elementos**
Podemos usar vários métodos para selecionar elementos:

#### `getElementById()`
Seleciona um elemento pelo seu `id`.
```javascript
const titulo = document.getElementById("titulo");
console.log(titulo.textContent); // "Olá, Mundo!"
```

#### `getElementsByClassName()`
Seleciona elementos por classe (retorna uma coleção).
```javascript
const paragrafos = document.getElementsByClassName("descricao");
console.log(paragrafos[0].textContent);
```

#### `querySelector()` e `querySelectorAll()`
Seleciona elementos usando seletores CSS.
```javascript
const titulo = document.querySelector("#titulo"); // Pega o primeiro que corresponder
const todosParagrafos = document.querySelectorAll(".descricao"); // Pega todos os correspondentes
```

---

### 🔸 **Modificando Elementos**
Podemos alterar o conteúdo e atributos dos elementos.

#### Modificar Texto (`textContent` e `innerHTML`)
```javascript
titulo.textContent = "Novo título!";
```
```javascript
titulo.innerHTML = "<span style='color:red'>Novo título!</span>";
```

#### Alterar Atributos (`setAttribute()` e propriedades diretas)
```javascript
titulo.setAttribute("class", "novo-estilo");
titulo.id = "novo-id";
```

#### Alterar Estilos (`style`)
```javascript
titulo.style.color = "blue";
titulo.style.fontSize = "24px";
```

---

### 🔸 **Criando e Removendo Elementos**
Podemos criar, adicionar e remover elementos dinamicamente.

#### Criar Elementos (`createElement()`)
```javascript
const novoParagrafo = document.createElement("p");
novoParagrafo.textContent = "Parágrafo dinâmico!";
document.body.appendChild(novoParagrafo);
```

#### Remover Elementos (`remove()`)
```javascript
titulo.remove(); // Remove o título da página
```

---

## 🔹 Eventos no DOM
O JavaScript permite que adicionemos interatividade ao DOM por meio de eventos.

Exemplo: Adicionar um evento de clique em um botão.
```html
<button id="meuBotao">Clique aqui</button>
```
```javascript
const botao = document.getElementById("meuBotao");

botao.addEventListener("click", function() {
    alert("Botão clicado!");
});
```

---

O **DOM** é essencial para manipular páginas web com **JavaScript**. Ele permite:
✅ Selecionar elementos  
✅ Modificar conteúdo e estilos  
✅ Criar e remover elementos dinamicamente  
✅ Responder a eventos do usuário  

É a base para criar interfaces dinâmicas e interativas na web! 🚀