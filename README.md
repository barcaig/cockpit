https://seuusuario.github.io/cockpit/# ⬡ Cockpit v0.7

Dashboard pessoal com 3 módulos: Profissional, Fitness e Financeiro.

## Deploy no GitHub Pages (2 minutos)

1. Crie um repo novo no GitHub (ex: `cockpit`)
2. Faça upload do `index.html` no repo (pode ser pelo próprio GitHub)
3. Vá em **Settings → Pages**
4. Em "Source", selecione **Deploy from a branch**
5. Selecione branch `main` e pasta `/ (root)`
6. Clique **Save**
7. Em ~1 minuto: `https://seuusuario.github.io/cockpit/`

## Primeiro uso

Ao abrir, o Cockpit pede sua **API key do Anthropic** para funcionalidades de IA:
- Pegue em [console.anthropic.com](https://console.anthropic.com/settings/keys)
- A key fica salva **apenas no localStorage** do seu navegador
- Pode pular se quiser usar só o Strava

## Módulos

### ⚡ Profissional
- **Gerador de Legendas**: Upload de gráficos → 3 opções de legenda para Twitter/X
- **Analisador de Documentos**: Upload de contratos/docs → análise com riscos e recomendações

### 🚴 Fitness
- **Strava**: Atividades reais, TSS, NP, HR
- **Zonas de Potência**: FTP 273W
- **Glicemia**: Registros manuais com alertas

### 💹 Financeiro
- **Câmbio**: USDC/USDT + pesquisa livre (qualquer moeda/ativo)
- **Voos**: Pesquisa de menores preços por rota

## Tecnologia
- HTML puro, zero dependências, zero build
- API Anthropic (Claude Sonnet) com `anthropic-dangerous-direct-browser-access`
- Strava OAuth + API v3
- Responsivo (mobile-first)
- PWA-ready (meta tags para home screen)
