# 🃏 Canastra Score - PWA

Marcador de pontos para Canastra com reconhecimento de cartas por foto usando IA (Google Gemini).

## 📱 Funcionalidades

- ✅ **Placar em tempo real** - Nós vs Eles até 3000 pontos
- ✅ **Histórico completo** - Todas as rodadas com opção de editar/excluir
- ✅ **Quem bateu** - Marca automaticamente +100 pontos
- ✅ **100% Offline** - Marcação manual funciona sem internet
- ✅ **Persistência local** - Dados salvos no dispositivo
- ✅ **Instalável** - Pode ser instalado como app
- 📷 **Reconhecimento por foto** - Conta cartas automaticamente usando IA

## 🤖 Configuração do Reconhecimento por Foto

O app usa o **Google Gemini** (gratuito) para reconhecer cartas. O usuário precisa obter uma chave API:

### Passo a passo (já guiado no app):
1. Abrir o app e clicar em ⚙️ ou no botão "CONFIGURAR PARA USAR FOTO"
2. Clicar em "Obter Chave Gratuita"
3. Fazer login com conta Google
4. Clicar em "Create API Key"
5. Copiar a chave e colar no app

**Custo:** 100% GRATUITO - até 1500 fotos por dia!

## 🚀 Deploy

### GitHub Pages (Recomendado)
1. Crie um repositório no GitHub
2. Faça upload de todos os arquivos
3. Vá em **Settings > Pages**
4. Selecione branch `main`, pasta `/ (root)`
5. Acesse pelo link gerado

### Netlify/Vercel
Arraste a pasta para o painel.

### Servidor Local
```bash
python -m http.server 8000
# ou
npx serve .
```

## 📸 Regras de Pontuação

| Item | Pontos |
|------|--------|
| Canastra Limpa (7+ cartas sem coringa) | 200 |
| Canastra Suja (7+ cartas com coringa) | 100 |
| Bater a rodada | 100 |
| Cartas 3, 4, 5, 6, 7 | 5 cada |
| Cartas 8, 9, 10, J, Q, K | 10 cada |
| Cartas A, 2, Coringa | 20 cada |

## 📁 Arquivos

```
canastra/
├── index.html      # App completo
├── manifest.json   # Config PWA
├── sw.js           # Service Worker
├── icon-192.png    # Ícone
├── icon-512.png    # Ícone
└── README.md
```

## 📲 Instalar no Celular

1. Acesse o app pelo navegador Chrome
2. Menu (⋮) > "Adicionar à tela inicial"
3. Pronto!

---

Feito para jogadores de Canastra 🃏
