# ImpactoCont Online

Esta é a versão online profissional do projeto, pensada para abrir por link em Windows, iPhone e Android.

## O que mudou
- Exportação de PDF feita no servidor (`/api/export-pdf`), sem usar `window.print()`.
- PDF em formato A4 com fundo e layout preservados.
- Logo embutido no HTML, então não some.
- Em `Contratos Fechados`, 1 clique seleciona e 2 cliques abre em nova página (`?view=id`).
- As cuotas só aparecem quando existe data da cuota.
- Se houver apenas 1 pagamento com data, ele aparece como `1ª cuota`.

## Como rodar
1. Instale Node.js 20 ou superior.
2. Na pasta do projeto, execute:
   ```bash
   npm install
   npm start
   ```
3. Abra no navegador:
   `http://localhost:3000`

## Como publicar na internet
Você pode publicar em Render, Railway ou outro serviço Node.

### Render
- Crie um novo `Web Service`.
- Envie esta pasta para um repositório GitHub.
- Build command: `npm install`
- Start command: `npm start`

## Observação sobre escolher nome/local
- Em navegadores Chromium compatíveis, o botão Exportar PDF tenta abrir a escolha de nome/local.
- Quando isso não for suportado, o navegador baixa o arquivo com o nome do contrato.
