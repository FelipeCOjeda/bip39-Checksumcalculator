# Calculadora de Checksum BIP39

Calcule a palavra final (checksum) da sua seed BIP39 de forma offline e segura.

## Arquivos

### `bip39_checksum_offline.html`
Versão 100% offline em arquivo único. Abra direto no navegador — não precisa de servidor, internet ou instalação.

**Funcionalidades:**
- 10 idiomas BIP39 (English, Español, Français, Italiano, Português, Čeština, 日本語, 한국어, 简体中文, 繁體中文)
- Autocomplete das palavras da wordlist
- Mostra todas as checksums válidas (128 para 12 palavras, 8 para 24 palavras)
- Análise de padrões (palavras repetidas, índices sequenciais, ordem alfabética)
- Nota de entropia 0–10
- SHA-256 nativo do navegador (`crypto.subtle`)

### `Calculadora BIP39.zip`
Versão original com interface premium (index.html + style.css + app.bundle.js). Descompacte e abra `index.html` no navegador.

## Como usar

1. **Desconecte completamente o dispositivo da internet** (Wi-Fi, cabo e Bluetooth).
2. Abra o HTML no navegador.
3. Selecione o idioma e o tamanho da seed (12 ou 24 palavras).
4. Digite as palavras de entropia (11 para seed de 12, ou 23 para seed de 24).
5. Preencha os bits extras de entropia (moedas cara/coroa).
6. Clique em **Calcular checksum**.
7. O resultado mostra:
   - **Suas palavras** — a seed parcial digitada.
   - **Checksums possíveis** — todas as palavras finais válidas. Clique em uma para completar a seed.

## Segurança

> **Nunca insira uma seed que proteja fundos reais em um dispositivo conectado à internet.**

Esta ferramenta é para uso educativo e geração de seeds novas em ambiente totalmente offline.

## Fonte da wordlist

Lista oficial BIP39: [github.com/bitcoin/bips](https://github.com/bitcoin/bips/blob/master/bip-0039)

## Licença

MIT
