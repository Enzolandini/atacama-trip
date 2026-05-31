# Atacama 2025 - App de Viagem

App PWA para organizar os documentos da viagem ao Deserto do Atacama (9 a 17 de agosto de 2025).

---

## Como instalar no Android

1. Hospede o arquivo `index.html` online (opcoes gratuitas abaixo)
2. Abra o link no **Google Chrome** do seu Android
3. Toque nos **3 pontos** no canto superior direito
4. Selecione **"Adicionar a tela inicial"**
5. O app aparece como icone na tela inicial, igual a um app nativo

---

## Como hospedar gratuitamente

### Opcao 1 — Netlify Drop (mais facil, sem cadastro)
1. Acesse [drop.netlify.com](https://app.netlify.com/drop)
2. Arraste a pasta `atacama-travel-app` para a pagina
3. Copie o link gerado e abra no Chrome do Android

### Opcao 2 — GitHub Pages
1. Crie um repositorio no GitHub
2. Envie os arquivos `index.html` e `manifest.json`
3. Va em Settings > Pages > selecione a branch `main`
4. Acesse o link `https://seu-usuario.github.io/nome-do-repo`

---

## Funcionalidades

- Documentos organizados por dia (9 a 17 de agosto)
- 3 categorias: **Passagens**, **Passeios**, **Seguro**
- Selecao especifica dos 4 voos:
  - GRU -> SCL (Sao Paulo - Santiago)
  - SCL -> CJC (Santiago - Calama)
  - CJC -> SCL (Calama - Santiago)
  - SCL -> GRU (Santiago - Sao Paulo)
- Upload de PDF ou imagem para cada documento
- Visualizacao de arquivos dentro do proprio app
- Campo de observacoes por documento (horario, ponto de encontro, etc.)
- Multiplos passeios por dia
- Funciona offline apos o primeiro acesso
- Todos os arquivos salvos localmente no aparelho

---

## Arquivos

```
atacama-travel-app/
  index.html      — app completo (HTML + CSS + JS em um unico arquivo)
  manifest.json   — configuracao PWA para instalacao no Android
  README.md       — este arquivo
```

---

## Observacoes

- Os documentos sao salvos no **IndexedDB** do navegador, diretamente no aparelho. Nenhum dado e enviado para servidores externos.
- Nao desinstale o Chrome nem limpe os dados do navegador para nao perder os documentos salvos.
- Para backup, salve os PDFs originais em outro lugar tambem.
