# Calculadora de Ponto

Aplicativo web simples, em HTML/CSS/JS puro, para registrar horas trabalhadas ao longo do mês e gerar um espelho de ponto em PDF — com cálculo opcional de hora extra, banco de horas e pagamento.

**Acesse online:** https://ludmilajohnston.github.io/calculadora-ponto/

## Funcionalidades

- **Registro diário de horas** para todos os dias do mês selecionado, com opção de ocultar sábados e domingos.
- **Intervalo de almoço** configurável: sem intervalo, um horário por dia ou um único horário fixo para o mês inteiro.
- **Hora extra**: define a partir de quantas horas por dia ela é contada e o multiplicador aplicado (ex: 1,5x).
- **Banco de horas**: compara as horas trabalhadas com a carga horária esperada e mostra o saldo (positivo ou devido).
- **Cálculo de pagamento**: aplica um valor por hora (em qualquer moeda) sobre o total de horas.
- **Formato de hora** 24h ou 12h (AM/PM).
- **Nota personalizada** que pode ser incluída no PDF gerado.
- **Exportação em PDF**, com opção de usar folha timbrada da AYIO ou folha branca.

Nenhum campo é obrigatório — o app se adapta às opções marcadas.

## Como usar

1. Abra o link acima (ou o `index.html` localmente).
2. Preencha o nome do ponto e o mês de referência.
3. Marque as opções avançadas que quiser usar (intervalo, hora extra, pagamento, banco de horas, nota).
4. Preencha o registro de horas de cada dia.
5. Clique em **Calcular** para ver os totais e depois em **Salvar PDF** para exportar.

## Rodando localmente

Basta abrir o `index.html` em um navegador — não é necessário servidor nem instalação. Mantenha os três arquivos (`index.html`, `style.css`, `script.js`) na mesma pasta, pois o app não depende de nada além deles (a folha timbrada já vem embutida em base64 no `script.js`).

## Estrutura do projeto

| Arquivo | Descrição |
|---|---|
| `index.html` | Estrutura e campos da página |
| `style.css` | Estilos visuais |
| `script.js` | Toda a lógica de cálculo e geração do PDF |

Geração de PDF via [jsPDF](https://github.com/parallax/jsPDF) e [html2canvas](https://github.com/niklasvh/html2canvas), carregados via CDN.

## Publicando no GitHub Pages

1. Faça o fork ou clone deste repositório (ou crie um novo com os 3 arquivos na raiz).
2. Vá em **Settings > Pages**.
3. Em "Source", selecione a branch `main`/`master` e a pasta `/ (root)`.
4. Salve. Em alguns minutos o app estará disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.
