# Plataforma UniForma

A **Plataforma UniForma** é uma aplicação web desenvolvida para apoiar atividades acadêmicas e processos de formação vinculados à **Universidade Estadual de Montes Claros (Unimontes)**.

O sistema busca facilitar a organização, submissão, acompanhamento e gerenciamento de demandas formativas, oferecendo diferentes recursos para usuários e responsáveis pela gestão da plataforma.

Este repositório corresponde a um **fork do projeto original da Plataforma UniForma**, utilizado para desenvolvimento, acompanhamento e registro das minhas contribuições ao sistema.

---

## Funcionalidades

Entre as funcionalidades da plataforma estão:

- Cadastro e autenticação de usuários;
- Gerenciamento de perfis e permissões;
- Submissão de propostas;
- Acompanhamento das submissões realizadas;
- Visualização e gerenciamento de submissões;
- Processo de curadoria e avaliação;
- Registro de interesses em atividades;
- Sistema de votos;
- Pesquisa de submissões;
- Filtros para facilitar a localização e organização dos registros;
- Diferentes funcionalidades de acordo com o perfil e permissões do usuário.

---

## Tecnologias utilizadas

O projeto utiliza principalmente:

- **PHP**
- **Laravel**
- **Blade**
- **JavaScript**
- **HTML**
- **CSS**
- **Banco de dados relacional**
- **Git**
- **GitHub**

O framework Laravel é utilizado para a implementação da aplicação web, organização das rotas, controllers, models, repositories, regras de negócio e comunicação com o banco de dados.

---

## Estrutura do projeto

A aplicação segue a organização fornecida pelo Laravel, incluindo diretórios responsáveis por diferentes partes do sistema.

```text
app/
├── Http/
│   ├── Controllers/
│   └── Requests/
│
├── Models/
│
├── Repositories/
│   └── Eloquent/
│
resources/
├── views/
│
routes/
├── web.php
│
database/
├── migrations/
```

### Controllers

Responsáveis por receber as requisições realizadas pela aplicação e coordenar o fluxo entre as diferentes camadas do sistema.

### Models

Representam as entidades da aplicação e realizam a comunicação com o banco de dados por meio do Eloquent ORM.

### Repositories

Utilizados para organizar as consultas e operações relacionadas aos dados da aplicação, separando parte da lógica de acesso aos dados dos controllers.

### Views

Contêm as páginas e componentes responsáveis pela interface apresentada ao usuário.

### Routes

Definem as URLs disponíveis na aplicação e direcionam cada requisição para seu respectivo controller.

---

## Minhas contribuições

Este fork é utilizado para registrar as funcionalidades e melhorias desenvolvidas durante minha participação no projeto.

Entre as atividades realizadas estão:

- Desenvolvimento e manutenção de funcionalidades da plataforma;
- Implementação de funcionalidades utilizando Laravel;
- Alterações em controllers, repositories e views;
- Melhorias na interface de submissões;
- Implementação de pesquisa de submissões por título;
- Implementação e aperfeiçoamento de filtros;
- Integração dos filtros entre frontend e backend;
- Correções e melhorias no fluxo de consulta das submissões;
- Utilização de Git e GitHub para versionamento do código;
- Desenvolvimento em branch própria e envio das alterações para revisão por meio de Pull Requests.

---

## Pesquisa e filtros

Uma das melhorias implementadas na plataforma envolve o sistema de pesquisa e filtragem das submissões.

A funcionalidade permite que os registros sejam consultados de acordo com parâmetros enviados pela interface, como termos de pesquisa e filtros disponíveis.

No backend, as consultas são realizadas utilizando os recursos do **Eloquent ORM**, permitindo combinar condições de pesquisa com paginação e relacionamentos entre as entidades.

Exemplo simplificado do fluxo:

```text
Usuário seleciona um filtro
          ↓
Interface envia os parâmetros
          ↓
Controller recebe a requisição
          ↓
Repository aplica os filtros
          ↓
Consulta é realizada no banco
          ↓
Resultados são paginados
          ↓
Interface exibe as submissões encontradas
```

Essa estrutura permite manter a lógica de consulta organizada e facilita futuras melhorias no sistema de pesquisa.

---

## Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/ellenloui/plataforma_uniforma.git
```

Entre na pasta do projeto:

```bash
cd plataforma_uniforma
```

### 2. Instale as dependências do PHP

```bash
composer install
```

### 3. Instale as dependências do frontend

```bash
npm install
```

### 4. Configure o ambiente

Crie o arquivo `.env` a partir do arquivo de exemplo:

```bash
cp .env.example .env
```

No Windows, o arquivo também pode ser copiado manualmente.

Configure no `.env` as informações necessárias para o banco de dados e demais serviços utilizados pela aplicação.

### 5. Gere a chave da aplicação

```bash
php artisan key:generate
```

### 6. Execute as migrations

```bash
php artisan migrate
```

### 7. Execute o frontend

```bash
npm run dev
```

### 8. Inicie a aplicação

```bash
php artisan serve
```

Por padrão, a aplicação poderá ser acessada em:

```text
http://127.0.0.1:8000
```

---

## Versionamento

Durante o desenvolvimento são utilizados **Git e GitHub** para controle de versão.

As alterações deste fork são desenvolvidas principalmente na branch:

```text
develop-v2
```

Fluxo utilizado:

```text
Projeto original
      ↓
Fork pessoal
      ↓
Branch de desenvolvimento
      ↓
Alterações
      ↓
Commit
      ↓
Push
      ↓
Pull Request
```

---

## Repositório original

Este projeto é baseado no repositório da **Plataforma UniForma**.

Repositório original:

```text
uniforma/plataforma_uniforma
```

Este fork mantém as alterações e contribuições realizadas durante minha participação no desenvolvimento da plataforma.

---

## Autoria e contribuição

**Ellen Louise Freitas Santos**

Desenvolvimento e contribuição na Plataforma UniForma, incluindo implementação de funcionalidades, manutenção do sistema, melhorias no fluxo de submissões e desenvolvimento de mecanismos de pesquisa e filtragem.

---

## Observação

A Plataforma UniForma é um projeto desenvolvido de forma colaborativa. Este repositório não representa autoria exclusiva da aplicação, mas registra as contribuições realizadas por mim durante o desenvolvimento do projeto.
