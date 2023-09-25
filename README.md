# [Blog de jogos](https://lucasll0.github.io/Projeto/) 

## 📌 Sobre o trabalho:
Este trabalho fez uso da jamstack Jekyll, para gerar um site estático, implementando diferentes ações de workflow e usar os princípios básico de gerencionameto de versões.

### Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- [Ruby 3.1.4](https://www.ruby-lang.org/en/downloads/)
- [Jekyll](https://jekyllrb.com/docs/)

## Criação e clonagem do repositório:

Estes foram os passos para a criação deste repositório, além da instalação do Jekyll, que pode ser verificada [aqui.](https://jekyllrb.com/docs/installation/)

![img0](imagem da criação de repositório)

Para a clonagem de repositório, deve-se inserir o seguinte comando:
```
git clone
```
seguido do url do seu repositório, como no exemplo a seguir:
```
git clone https://github.com/lucasll0/Projeto.git
```
Entre no diretório que foi clonado:
```
cd lucasll0.github.io
```
E então desenvolva a estrutura do site de acordo com o necessário.

## Uso do GitHub Actions:
O GitHub Actions é um serviço de automação de fluxo de CI/CD fornecido pelo GitHub. Ele permite que os desenvolvedores automatizem tarefas como compilação, teste e implantação de código.

###### Trabalhos: São grupos de tarefas que você configura para serem executadas.

#### Criação do arquivo: Para começar, crie um arquivo .github/workflows/nome-do-fluxo.yml no seu repositório. Este arquivo contém as instruções para o GitHub Actions sobre o que fazer quando um evento ocorre.

**Fluxos de trabalho**: São definidos em arquivos YAML no diretório .github/workflows. Eles são acionados por eventos específicos, como abrir uma solicitação de pull ou fazer um envio (push) de código.

**Execução**:  Quando o evento desejado acontece, o GitHub Actions inicia automaticamente o fluxo de trabalho, seguindo as etapas que você definiu no arquivo YAML.

**Ação**: Durante a execução, você pode usar ações, que são conjuntos de comandos pré-definidos, para realizar tarefas específicas, como construir um site. Por exemplo, ao criar um site estático com Jekyll, você pode usar uma ação especializada para essa finalidade.

**Ação de Teste**: Pós a construção do site, você deve adicionar uma ação de teste para verificar se o site foi criado corretamente e atende aos padrões de qualidade definidos.

**Implantação Automática**: Para implantar o site, você configura um ambiente de implantação, que pode ser um servidor de hospedagem como o GitHub Pages. Dentro desse ambiente, você utiliza outra ação para efetuar a implantação, enviando os arquivos gerados durante a construção para o servidor do GitHub Pages.

Neste repositório estão presente os seguintes fluxos de trabalho:

![image](https://github.com/el1ziane/el1ziane.github.io/assets/113150368/7960e97e-2bb0-4fa1-aa39-4faf2d935a2e)

## **ESLint**

Instalação:

![Captura de tela 2023-09-17 093955](imagem de instalação através do VSCode)

Realizando a configuração em: `⚙️settings`, pesquisando por ```“editor.codeActionsOnSave”```:

![Captura de tela 2023-09-20 173427](https://github.com/el1ziane/el1ziane.github.io/assets/113150368/25dfbe04-81b4-482d-b21c-2b4ff081cb82)

No terminal será necessário digitar:

```
npm install eslint --save-dev
```
Então

```
npx eslint –-init
```
Em seguida, deve-se selecionar as opções de uso de acordo com o seu projeto.

Pacotes intalados no projeto!

[img0](Imagem de barra lateral esquerda)

## 🚀 Desafios

### **Arquivo de configuração** `.gitignore`:
Por estar utilizando Jekyll com `bundler`, foi necessário seguir a documentação do Jekyll e adicionar os seguintes arquivos ao `.gitignore`:
```
_site
.sass-cache
.jekyll-cache
.jekyll-metadata
vendor
.bundle/
```

### **Algum outro desafio**

![img4]()

### **Rebase Interativo**

![img2]()

### **Branch Protegida**

![img3]()


