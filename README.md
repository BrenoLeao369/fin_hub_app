# FluxoHUD — Organização Financeira Visual

Aplicativo de organização financeira pessoal com **HUD animada, visual e interativa**, desenvolvido em **Python**, projetado para substituir planilhas rígidas e cinzas por uma experiência autônoma, acolhedora e 100% sem código.

---

## Diferenciais e Funcionalidades

- **Motor de Tabelas Autônomas (Sem Código):** Crie múltiplos módulos financeiros (ex.: *Gastos Fixos*, *Cartão*, *Viagem*, *Metas*), defina colunas personalizadas e obtenha totais, subtotais e saldos automaticamente.
- **HUD Interativa com Imagens Próprias:** Adicione fotos de capa nos seus objetivos/tabelas e anexe comprovantes ou recibos diretamente nos lançamentos, com alternância de temas visuais (*Dark HUD*, *Light Clean*).
- **Calculadora de Juros Integrada:** Simule juros simples, juros compostos (com aporte inicial e mensal) e evolução de parcelamentos, podendo transformar simulações direto em metas de acompanhamento.
- **Local-First & Privado:** Todos os dados e imagens ficam salvos localmente no seu dispositivo via **SQLite**, funcionando offline e com total privacidade.

---

## Stack Tecnológica

- **Linguagem:** Python 3.11+
- **Interface Gráfica (UI):** Flet (baseado em Flutter, com suporte para Desktop, Web e empacotamento Android `.aab`)[cite: 1]
- **Banco de Dados:** SQLite (`sqlite3` nativo)[cite: 1]

---

## 📂 Estrutura do Projeto

```text
fin_hud_app/
├── assets/
│   └── user_media/      # Imagens locais do usuário (capas, comprovantes, ícones)
├── db/                  # Conexão SQLite, criação de tabelas e queries
├── models/              # Estruturas de dados (Tabela, Coluna, Lançamento, Simulação)
├── services/            # Motor de cálculos, juros e gerenciamento de mídia
├── ui/                  # Telas, temas e componentes animados da HUD
├── .gitignore
├── README.md
├── requirements.txt
└── main.py              # Ponto de entrada do aplicativo
```[cite: 1]

---

## 🚀 Como Executar Localmente

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/BrenoLeao369/fin_hud_app.git
   cd fin_hud_app