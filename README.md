# 🃏 Canastra Score - PWA

Marcador de pontos para Canastra com reconhecimento de cartas por foto usando IA.

## 📱 Funcionalidades

- ✅ **Placar em tempo real** - Nós vs Eles até 3000 pontos
- ✅ **Histórico completo** - Todas as rodadas com opção de editar/excluir
- ✅ **Quem bateu** - Marca automaticamente +100 pontos para o ganhador da rodada
- ✅ **100% Offline** - Funciona sem internet após instalado
- ✅ **Persistência local** - Dados salvos mesmo fechando o app
- ✅ **Instalável** - Pode ser instalado como app na tela inicial
- 📷 **Reconhecimento por foto** - Conta cartas automaticamente usando IA (requer internet)

## 🚀 Como Usar

### Opção 1: GitHub Pages (Recomendado)

1. Crie um repositório no GitHub
2. Faça upload de todos os arquivos
3. Vá em **Settings > Pages**
4. Selecione a branch `main` e pasta `/ (root)`
5. Acesse pelo link gerado (ex: `seuusuario.github.io/canastra`)

### Opção 2: Servidor Local

```bash
# Com Python
python -m http.server 8000

# Com Node.js
npx serve .

# Com PHP
php -S localhost:8000
```

Acesse `http://localhost:8000`

### Opção 3: Netlify/Vercel

Arraste a pasta para o painel do Netlify ou Vercel.

## 📸 Reconhecimento de Cartas

O app usa a API do Claude (Anthropic) para reconhecer cartas por foto. Esta funcionalidade:

- **Requer conexão com internet** para funcionar
- Identifica jogos e canastras automaticamente
- Calcula valores das cartas seguindo as regras oficiais

### Regras de Pontuação Reconhecidas

| Item | Pontos |
|------|--------|
| Canastra Limpa (7+ cartas sem coringa) | 200 |
| Canastra Suja (7+ cartas com coringa) | 100 |
| Bater a rodada | 100 |
| Cartas 3, 4, 5, 6, 7 | 5 cada |
| Cartas 8, 9, 10, J, Q, K | 10 cada |
| Cartas A, 2, Coringa | 20 cada |

## 📁 Estrutura de Arquivos

```
canastra/
├── index.html      # App principal (tudo inline)
├── manifest.json   # Configuração PWA
├── sw.js           # Service Worker (offline)
├── icon-192.png    # Ícone 192x192
├── icon-512.png    # Ícone 512x512
├── icon.svg        # Ícone vetorial
├── index.jsx       # Versão React (opcional)
└── README.md       # Este arquivo
```

## 💡 Dicas de Uso

1. **Para reconhecimento por foto**: Tire a foto com boa iluminação e cartas bem visíveis
2. **Cartas empilhadas**: O sistema identifica jogos mesmo com cartas sobrepostas
3. **Editar rodadas**: Clique no ✏️ para corrigir qualquer erro
4. **Novo jogo**: Use o botão "NOVO JOGO" para zerar tudo

## 🔧 Tecnologias

- HTML5 + CSS3 + JavaScript Vanilla
- Service Worker para funcionamento offline
- LocalStorage para persistência
- API Claude (Anthropic) para visão computacional
- PWA com manifest para instalação

## 📲 Instalar no Celular

1. Acesse o app pelo navegador (Chrome recomendado)
2. Toque no menu (⋮) do navegador
3. Selecione "Adicionar à tela inicial" ou "Instalar app"
4. Pronto! O app aparecerá como qualquer outro aplicativo

---

Feito com ❤️ para jogadores de Canastra
