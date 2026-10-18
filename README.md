# ⚔️ Escrevendo as Classes de um Jogo

Projeto desenvolvido como parte dos desafios práticos da [DIO (Digital Innovation One)](https://www.dio.me/), com o objetivo de praticar os conceitos fundamentais de JavaScript utilizando classes e objetos.

## 📌 Sobre o Projeto

O desafio consiste em criar uma classe genérica que represente um herói de uma aventura. Cada herói possui nome, idade e tipo, além de um método responsável por executar um ataque de acordo com sua classe.

O projeto utiliza estruturas de decisão para determinar o tipo de ataque realizado por cada herói.

## 🎯 Objetivos

* Praticar a criação de classes e objetos em JavaScript.
* Trabalhar com construtores e propriedades.
* Utilizar métodos para definir comportamentos.
* Aplicar estruturas condicionais para determinar os ataques.
* Utilizar variáveis, operadores e funções.
* Desenvolver a lógica de programação.

## 🛠️ Tecnologias Utilizadas

* **JavaScript**
* **Node.js** (para execução do projeto)
* **Git e GitHub** (para versionamento e armazenamento do código)

## 🧙 Funcionalidades

O projeto implementa uma classe chamada `Heroi`, com as seguintes propriedades:

| Propriedade | Descrição       |
| ----------- | --------------- |
| `nome`      | Nome do herói   |
| `idade`     | Idade do herói  |
| `tipo`      | Classe do herói |

A classe também possui o método `atacar()`, que exibe uma mensagem com o tipo do herói e seu respectivo ataque.

### ⚔️ Tipos de heróis e ataques

| Tipo de Herói | Ataque         |
| ------------- | -------------- |
| Mago          | Magia          |
| Guerreiro     | Espada         |
| Monge         | Artes marciais |
| Ninja         | Shuriken       |

## 💻 Exemplo de Execução

**Código:**

```javascript
class Heroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    atacar() {
        let ataque = "";

        switch (this.tipo.toLowerCase()) {
            case "mago":
                ataque = "magia";
                break;

            case "guerreiro":
                ataque = "espada";
                break;

            case "monge":
                ataque = "artes marciais";
                break;

            case "ninja":
                ataque = "shuriken";
                break;

            default:
                ataque = "um ataque desconhecido";
        }

        console.log(`O ${this.tipo} atacou usando ${ataque}`);
    }
}

const heroi1 = new Heroi("Gandalf", 100, "mago");
const heroi2 = new Heroi("Aragorn", 35, "guerreiro");
const heroi3 = new Heroi("Lee", 28, "monge");
const heroi4 = new Heroi("Hattori", 25, "ninja");

heroi1.atacar();
heroi2.atacar();
heroi3.atacar();
heroi4.atacar();
```

**Saída esperada:**

```text
O mago atacou usando magia
O guerreiro atacou usando espada
O monge atacou usando artes marciais
O ninja atacou usando shuriken
```

## ▶️ Como Executar o Projeto

### Pré-requisitos

* [Node.js](https://nodejs.org/) instalado.
* [Git](https://git-scm.com/) instalado, caso deseje clonar o repositório.

### Passo a passo

**1. Clone o repositório:**

```bash
git clone https://github.com/SEU-USUARIO/desafio-classes-jogo.git
```

**2. Acesse a pasta do projeto:**

```bash
cd desafio-classes-jogo
```

**3. Execute o arquivo JavaScript:**

```bash
node index.js
```

> **Observação:** substitua `SEU-USUARIO` pelo seu nome de usuário do GitHub e ajuste o nome do repositório, se necessário.

## 📚 Conceitos Praticados

Durante o desenvolvimento deste desafio, foram aplicados os seguintes conceitos:

* Classes e objetos.
* Construtor (`constructor`).
* Propriedades e métodos.
* Palavra-chave `this`.
* Estrutura de decisão `switch`.
* Operadores e variáveis.
* Template strings.
* Instanciação de objetos com `new`.

## 🚀 Aprendizados

Este projeto contribuiu para o desenvolvimento da lógica de programação e para a compreensão dos conceitos de orientação a objetos em JavaScript, demonstrando como diferentes objetos podem compartilhar a mesma estrutura e apresentar comportamentos específicos de acordo com suas propriedades.

## 👨‍💻 Autor

Desenvolvido por **Eduardo Machado**, como parte dos estudos de JavaScript e dos desafios práticos da DIO.

🔗 **GitHub:**(https://github.com/edusilverfit)

---

⭐ Se este projeto foi útil para você, considere deixar uma estrela no repositório!
