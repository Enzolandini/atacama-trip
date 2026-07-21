# Atacama 2026 - App de Viagem

App PWA para organizar a viagem ao Deserto do Atacama (9 a 17 de agosto de 2026), com base nos vouchers de passeios (Civitatis), apólices de seguro viagem (GTA/IZA) e transfer contratados.

---

## Abas do app

- **Cronograma** — roteiro dia a dia, do embarque no Brasil (9/08, 23h) até o voo de volta (17/08), com horário de retirada/duração de cada passeio e os intervalos livres entre eles.
- **Documentos** — apólices de seguro viagem (Enzo e Esther), contato de emergência 24h e material de telemedicina/scan facial. É possível adicionar outros documentos (ex: passagem aérea) pelo botão **+**.
- **Passeios** — voucher de cada passeio contratado (Valle de la Luna, Vale do Arco-íris, Observação de estrelas, Lagoa Cejar, El Tatio, Piedras Rojas, Rota dos Salares) e do transfer aeroporto ↔ San Pedro de Atacama, com ponto de encontro, fornecedor, valor e condições de cancelamento. O PDF original de cada voucher pode ser aberto direto no app.
- **Itens** — checklist do que levar em cada passeio + lista geral da viagem. Os itens marcados ficam salvos no aparelho.

---

## Como instalar no Android

1. Hospede a pasta do projeto online (opções gratuitas abaixo)
2. Abra o link no **Google Chrome** do seu Android
3. Toque nos **3 pontos** no canto superior direito
4. Selecione **"Adicionar a tela inicial"**
5. O app aparece como ícone na tela inicial, igual a um app nativo

---

## Como hospedar gratuitamente

### Opção 1 — Netlify Drop (mais fácil, sem cadastro)
1. Acesse [drop.netlify.com](https://app.netlify.com/drop)
2. Arraste a pasta do projeto para a página
3. Copie o link gerado e abra no Chrome do Android

### Opção 2 — GitHub Pages
1. Vá em Settings > Pages > selecione a branch `main`
2. Acesse o link `https://seu-usuario.github.io/nome-do-repo`

---

## Arquivos

```
atacama-trip/
  index.html                        — app completo (HTML + CSS + JS em um único arquivo)
  manifest.json                     — configuração PWA para instalação no Android
  assets/documentos/                — apólices de seguro (Enzo, Esther) e material de telemedicina
  assets/passeios/                  — vouchers originais de cada passeio e do transfer
  README.md                         — este arquivo
```

---

## Observações

- Os dados de cronograma, passeios e itens estão embutidos no código (`index.html`), extraídos diretamente dos vouchers e apólices fornecidos.
- Documentos adicionados manualmente pelo botão **+** ficam salvos no **IndexedDB** do navegador, direto no aparelho — nenhum dado é enviado para servidores externos.
- Horários de retirada dos passeios podem variar; os fornecedores confirmam o horário exato por WhatsApp na véspera de cada atividade.
- Não desinstale o Chrome nem limpe os dados do navegador para não perder os itens marcados e documentos extras adicionados.
