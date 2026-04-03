# 🐟 Pesqueiro Peroba — Sistema de Gestão v2.0

## 🔐 Acesso Padrão
| Campo    | Valor |
|----------|-------|
| Usuário  | `adm` |
| Senha    | `1`   |
| Perfil   | Administrador |

---

## ✅ Funcionalidades v2.0

### Operação
- [x] **Dashboard** — estatísticas em tempo real
- [x] **Comandas** — status: Aberta / Parcialmente Paga / Fechada (sem "em atendimento")
- [x] **Nova comanda** — nº, cliente, pescadores, visitantes nominais, tipo
- [x] **Adição de itens** — busca inteligente por sinônimos (energético → Monster, Red Bull...)
- [x] **Observação opcional** nos itens (não obrigatória)
- [x] **Botão "Adicionar Mais"** — sem sair da tela
- [x] **Visitantes nominais** — adicionar, editar, marcar como "saiu"
- [x] **Múltiplos pagamentos** — PIX, crédito, débito, dinheiro com calculadora
- [x] **🍳 Aba Cozinha** — pedidos pendentes de entrega, botão "✅ Entregue"
- [x] **🚪 Portaria** — conferência nominal, libera saída só se pago
- [x] **💰 Caixa** — abrir/fechar, por forma de pagamento, histórico de dias
- [x] **📈 Relatórios** — hoje/ontem/semana/mês/personalizado
- [x] **🖨️ Comprovante** — cupom completo para impressão/PDF

### Administração
- [x] **Produtos** — nome, categoria, preço, setor, sinônimos, ativo/inativo
- [x] **Usuários** — admin, garçom, caixa; ativar/desativar; redefinir senha
- [x] **Configurações** — valor da pescaria parametrizável, nome, endereço, CNPJ
- [x] **Exportar backup** — JSON com todos os dados

### Técnico
- [x] Dados persistidos em localStorage (não perdem ao fechar o browser)
- [x] Responsivo mobile + desktop
- [x] PWA (installável como app no celular)
- [x] Zero dependências externas
- [x] Deploy em Vercel/Netlify/Cloudflare em 1 clique

---

## 🚀 Deploy

### Netlify (mais rápido)
1. Acesse [netlify.com](https://netlify.com) → *Sites* → *Add new site*
2. **Arraste a pasta** diretamente para a área de drop
3. Pronto — URL gerada automaticamente

### Vercel
1. Acesse [vercel.com](https://vercel.com) → *New Project*
2. Faça upload da pasta ou conecte ao GitHub
3. Clique em *Deploy*

### Cloudflare Pages
1. Acesse [pages.cloudflare.com](https://pages.cloudflare.com)
2. *Create a project* → *Direct Upload*
3. Faça upload dos arquivos

---

## 📱 Instalar como App (PWA)

Após publicar o site:

**Android (Chrome):**
1. Abra o site no Chrome
2. Menu (⋮) → *Adicionar à tela inicial*

**iOS (Safari):**
1. Abra o site no Safari
2. Compartilhar (□↑) → *Adicionar à Tela de Início*

---

## 💰 Configurar Valor da Pescaria

1. Login como admin → **⚙️ Config**
2. Altere o campo **"Valor da Pescaria"**
3. Clique em **Salvar**
4. Toda nova comanda usará o valor atualizado

---

## 🗂 Estrutura de Arquivos

```
/
├── index.html      ← Sistema completo (único arquivo)
├── manifest.json   ← PWA manifest
├── icon-192.png    ← Ícone PWA (adicionar manualmente)
├── icon-512.png    ← Ícone PWA (adicionar manualmente)
└── README.md       ← Este arquivo
```

> **Nota sobre ícones:** Para uso como PWA, substitua os arquivos `icon-192.png` e `icon-512.png` pelo logo do Pesqueiro Peroba nos tamanhos indicados.

---

## 🔮 Estrutura Preparada Para

- **Impressão térmica** — cada produto tem campo `setor` e `imprime`
- **WhatsApp** — estrutura de dados pronta (ex: `C47 1 coca lata`)
- **Integração com API** — toda lógica separada em funções claras

---

*Pesqueiro Peroba • Jandira – SP • Sistema v2.0*
