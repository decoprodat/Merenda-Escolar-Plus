# 🍲 Merenda Plus

Sistema web de gestão de merenda escolar para escolas públicas, desenvolvido em grupo no primeiro semestre de 2026 como Trabalho Interdisciplinar do curso de TI da PUC Minas.

O Merenda Plus substitui o controle manual (anotações em papel e planilhas soltas) por uma plataforma única onde a **direção da escola** e as **merendeiras** registram e acompanham o estoque de alimentos, os cardápios, o preparo e o consumo das refeições, reduzindo o desperdício e a falta de insumos.

🔗 **Acesse o sistema:** _(link do deploy — em breve)_

> ℹ️ O sistema está hospedado em um plano gratuito: o primeiro acesso pode levar cerca de 1 minuto para carregar.

---

## ✨ Funcionalidades

**Para a diretora**
- Painel inicial com indicadores de consumo, estoque e problemas reportados
- Gestão do estoque: cadastro e remoção de alimentos, total de itens, alerta de baixo estoque e de produtos próximos do vencimento
- Planejamento de cardápios
- Central de alertas e reportes de problemas enviados pelas merendeiras
- Relatórios mensais de refeições servidas e desperdício (com gráficos)
- Gestão de usuários, incluindo aprovação de novos cadastros

**Para a merendeira**
- Consulta e busca no estoque, com destaque para itens perto da validade
- Visualização do cardápio do dia
- Registro do preparo das refeições e dos alimentos utilizados
- Registro de consumo, com cálculo automático do percentual de desperdício
- Envio de reportes de problemas (falta de alimento, equipamento quebrado, entregas etc.)

**Login com perfis de acesso:** cada usuário entra como diretora ou merendeira e só vê as telas do seu perfil. Novos cadastros ficam pendentes até a aprovação da direção.

---

## 🧑‍💻 Minha contribuição

Neste projeto fui responsável por:

- **Sistema de login e controle de acesso por perfil** (diretora / merendeira), incluindo cadastro de novos usuários com status pendente
- **Módulo de estoque da diretora:** listagem, cadastro e remoção de alimentos, indicadores de total de itens e baixo estoque, e alerta visual de produtos vencidos ou próximos do vencimento
- **Módulo de estoque da merendeira:** consulta paginada, busca de alimentos e lista de validades próximas

---

## 🛠️ Tecnologias

- **Front-end:** HTML5, CSS3, JavaScript (vanilla), Bootstrap 5, Bootstrap Icons, Chart.js
- **Back-end:** Node.js com [JSON Server](https://github.com/typicode/json-server) (API REST simulada a partir de um arquivo JSON)
- **Metodologia:** Design Thinking (personas, mapa de stakeholders, matriz CSD, proposta de valor, wireframes e user flows) e Scrum

---

## 🚀 Como executar localmente

Pré-requisito: [Node.js](https://nodejs.org/) instalado.

```bash
git clone https://github.com/decoprodat/Merenda-Escolar-Plus.git
cd Merenda-Escolar-Plus/codigo
npm install
npm start
```

Depois, acesse **http://localhost:3000** no navegador.

### Usuários de demonstração

| Login | Senha | Perfil |
|---|---|---|
| `diretora` | `123` | Diretora |
| `merendeira` | `123` | Merendeira |
| `admin` | `123` | Diretora e merendeira |

> Todos os dados do sistema são fictícios e servem apenas para demonstração.

---

## 📁 Estrutura do projeto

```
Merenda-Escolar-Plus/
├── codigo/
│   ├── db/db.json          # Base de dados (JSON Server)
│   ├── index.js            # Servidor Node.js
│   ├── package.json
│   └── public/             # Front-end
│       ├── assets/         # CSS, JavaScript e imagens
│       └── modulos/
│           ├── login/
│           ├── diretora/
│           └── merendeira/
└── docs/                   # Documentação (Design Thinking, wireframes, personas)
```

A documentação completa do processo de concepção está em [`docs/README.md`](docs/README.md).

---

## 👥 Equipe

- [André Luiz Pinheiro Lopes](https://github.com/decoprodat)
- [Davi Lavalle Carneiro](https://github.com/davicarneiro1558195-sys)
- [Gabriel Tavares Pandino](https://github.com/gabrielpandino-puc)
- [Gustavo Alves Costa Sousa](https://github.com/alvespcrl)


**Professores orientadores (PUC Minas):** Cleiton Silva Tavares, Diego Augusto de Faria Barros, Rommel Vieira Carneiro e Roselene Henrique Pereira Costa.
