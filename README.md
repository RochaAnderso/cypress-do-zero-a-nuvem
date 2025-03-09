# Cypress do Zero à Nuvem: Comandos Customizados, Boas Práticas e Aprendizados em Testes Automatizados

## **Introdução**

Neste projeto, exploramos o uso de comandos customizados no Cypress para otimizar testes automatizados, abordando a implementação de cy.dataTest e boas práticas aprendidas no curso "Cypress, do Zero à Nuvem". O foco é garantir testes mais claros, estáveis e fáceis de manter, com dicas para uma automação de testes mais robusta e confiável.

Este projeto foi desenvolvido como parte do curso **"Cypress, do Zero à Nuvem"** da escola online **Talking About Testing**, ministrado por **Walmyr Lima e Silva Filho**.

## **Requisitos Prévios**

Para executar este projeto, é necessário ter o **Node.js** e o **npm** instalados.

- **Node.js**: v18.15.0 ou superior
- **npm**: v9.5.0 ou superior

> É recomendável utilizar essas versões ou superiores para garantir a compatibilidade e bom funcionamento do projeto.

---

## **Instalação**

### **Windows**

1. Instale o Node.js e npm [aqui](https://nodejs.org/).
2. Clone este repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   ```
3. Acesse o diretório do projeto:
   ```bash
   cd nome-do-projeto
   ```
4. Instale as dependências de desenvolvimento:
   ```bash
   npm install
   ```
   ou, para a versão curta:
   ```bash
   npm i
   ```

### **Linux e macOS**

1. Instale o Node.js e npm via terminal:
   ```bash
   sudo apt install nodejs npm  # Para Linux (Ubuntu/Debian)
   brew install node            # Para macOS (Homebrew)
   ```
2. Clone este repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   ```
3. Acesse o diretório do projeto:
   ```bash
   cd nome-do-projeto
   ```
4. Instale as dependências de desenvolvimento:
   ```bash
   npm install
   ```

---

## **Configuração**

Antes de executar os testes, faça uma cópia do arquivo `cypress.env.example.json` e renomeie para `cypress.env.json`.

> **Importante:** No mundo real, você deve atualizar este arquivo com credenciais válidas. O arquivo `cypress.env.json` está listado no `.gitignore`, portanto, suas informações confidenciais estarão seguras e não serão versionadas.

---

## **Execução dos Testes**

- Para rodar os testes em modo **headless** (sem interface gráfica):

  ```bash
  npm test
  ```

  ou, para a versão curta:

  ```bash
  npm t
  ```

- Para abrir o Cypress no modo **interativo**:

  ```bash
  npm run cy:open
  ```

---

## **O que Você Vai Aprender com o Curso**

Durante o curso **Cypress, do Zero à Nuvem**, você aprenderá conceitos fundamentais para escrever testes mais claros, eficientes e confiáveis. Alguns dos principais aprendizados incluem:

- Encadeamento de comandos no Cypress
- Uso de re-tentativas para garantir maior estabilidade dos testes
- Interação com campos de seleção suspensa
- Aplicação de comandos customizados para manter os testes mais organizados e legíveis
- Estruturação adequada dos testes para maior clareza e manutenção
- Organização de fixtures e utilização correta de `beforeEach()` para preparar o ambiente de testes

Esses conhecimentos serão fundamentais para aprimorar suas habilidades em QA e automação de testes.

---

## **Dicas e Boas Práticas**

### **Boas Práticas:**

✅ Utilize comandos customizados como `cy.dataTest` para tornar seus testes mais limpos e fáceis de manter.\
✅ Utilize o comando `beforeEach()` para preparar o ambiente de teste e evitar repetições desnecessárias.\
✅ Faça uso de `aliases` e `fixtures` para manter o código mais organizado e evitar hardcodes.\
✅ Escreva descrições claras e objetivas para seus testes e utilize `it.only()` ou `it.skip()` com moderação.\
✅ Mantenha suas dependências atualizadas para evitar problemas de compatibilidade.

### **Más Práticas (Evite):**

❌ Evite interagir diretamente com elementos utilizando seletores frágeis, como `nth-child` ou classes genéricas.\
❌ Não utilize `cy.wait()` com tempos fixos excessivos; utilize comandos que aguardam automaticamente as respostas da API ou renderização dos elementos.\
❌ Evite repetir código desnecessariamente; crie comandos customizados sempre que possível.\
❌ Não utilize `.then()` para encadear ações simples quando puder confiar no comportamento automático de re-tentativas do Cypress.

---

## **Créditos**

Este projeto foi desenvolvido como parte do curso **"Cypress, do Zero à Nuvem"**, ministrado por **Walmyr Lima e Silva Filho** na plataforma **Talking About Testing**.

---

## **Contato**

Caso tenha alguma dúvida ou sugestão, fique à vontade para abrir uma issue ou contribuir diretamente com melhorias para o projeto.

---

Esta documentação foi criada por **Francisco Anderson Rocha de Sousa** durante as aulas do curso **"Cypress, do Zero à Nuvem"**.

**Happy Testing! 🚀**

