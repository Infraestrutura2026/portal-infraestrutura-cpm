# Portal de Sistemas — Complexo Penal de Marília

Portal de acesso aos sistemas do **Núcleo de Infraestrutura e Logística** do Complexo Penal de Marília (Polícia Penal — Governo do Estado de São Paulo).

## 🔗 Sistemas disponíveis

| # | Sistema | Descrição | Link |
|---|---------|-----------|------|
| 1 | Controle de Saídas | Movimentação de PPL · Portaria — registro e consulta das saídas dos PPL's | https://controle-de-transito.vercel.app |
| 2 | Gestão de Estoque e Controle de Ferramentas | Almoxarifado · Ferramental — controle do estoque e do uso de ferramentas | https://ferramentas-e-estoque.vercel.app |
| 3 | **Gestão de Frota (Frota Pro v3.1)** | Veículos · Abastecimento · Manutenção — gerenciamento da frota | **https://frotacpm.vercel.app** |

> ⚠️ O cartão **Gestão de Frota** foi atualizado para apontar ao endereço novo
> (`https://frotacpm.vercel.app`). Antes apontava para o GitHub Pages
> (`https://infraestrutura2026.github.io/Frota`), que não é mais o endereço oficial.

## 📁 Estrutura

```
portal-infraestrutura-cpm/
├── index.html                      # Página única do portal (HTML + CSS + JS embutidos)
├── images/
│   └── brasao-policia-penal-sp.png # Brasão oficial da Polícia Penal de SP
├── DEPLOY-VERCEL.md                # Passo a passo para publicar/atualizar na Vercel
└── README.md
```

## 🚀 Publicação

A página é 100% estática (sem build). Veja o guia completo em
[`DEPLOY-VERCEL.md`](DEPLOY-VERCEL.md) para conectar este repositório à Vercel e
publicar em `https://portal-infraestrutura-cpm.vercel.app`.
