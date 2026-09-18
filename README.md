<h1 align="center">Conversão de Temperatura</h1>

<p align="center">
  <b>API/web app Node.js + Express para conversão entre Celsius e Fahrenheit</b><br>
  <sub>Projeto de estudo — documentação Swagger e testes automatizados</sub>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black" alt="Swagger" />
  <img src="https://img.shields.io/badge/Mocha-8D6748?style=for-the-badge&logo=mocha&logoColor=white" alt="Mocha" />
</p>

---

## 📝 Visão geral

Aplicação **Node.js + Express** que converte temperaturas entre **Celsius** e **Fahrenheit**. Desenvolvido como projeto de estudo (trilha KubeDev), serve de base para praticar containerização e deploy em **Kubernetes**.

Apesar de simples, o projeto cobre uma stack completa de backend: rotas Express, views com EJS, **documentação de API com Swagger** e **testes automatizados** com Mocha/Chai.

## 🔧 Funcionalidades

- Conversão **Celsius → Fahrenheit** e **Fahrenheit → Celsius**
- Interface web renderizada com **EJS**
- Documentação interativa da API via **Swagger UI** (`swagger.yaml`)

A lógica de conversão:

```js
celsiusFahrenheit = (v) => (v * 9) / 5 + 32
fahrenheitCelsius = (v) => ((v - 32) * 5) / 9
```

## 🛠️ Stack

| Camada | Tecnologia |
|--------|-----------|
| Backend | Node.js · Express |
| Views | EJS |
| Documentação | Swagger (swagger-ui-express) |
| Testes | Mocha · Chai |

## ⚙️ Como executar

**Pré-requisitos:** Node.js 18+ e npm.

```bash
# Clonar
git clone https://github.com/theeedu/convertation-temperature.git
cd convertation-temperature

# Instalar dependências
npm install

# Iniciar o servidor
node server.js
```

Acesse a aplicação em `http://localhost:3000` e a documentação Swagger na rota `/api-docs`.

## 📂 Estrutura

```
convertation-temperature/
├── convert.js         # Lógica de conversão
├── server.js          # Servidor Express
├── config/            # Configuração
├── views/             # Templates EJS
├── swagger.yaml       # Especificação da API
└── test/              # Testes (Mocha/Chai)
```

---

<p align="center">
  <sub>Projeto de estudo — Node.js, Express e Kubernetes (KubeDev)</sub>
</p>
