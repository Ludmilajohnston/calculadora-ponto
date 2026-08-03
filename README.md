# Calculadora de Ponto

App em HTML/CSS/JS puro (arquivos separados) para calcular horas trabalhadas, hora extra, banco de horas e pagamento mensal, com exportação em PDF (com ou sem a folha timbrada da AYIO).

## Arquivos
- `index.html` — estrutura da página
- `style.css` — estilos
- `script.js` — toda a lógica (inclui o timbrado embutido em base64, não precisa de imagem separada)

## Como rodar localmente
Abra o `index.html` no navegador (mantenha os 3 arquivos na mesma pasta).

## Como publicar no GitHub Pages
1. Crie um repositório novo no GitHub (ex: `calculadora-ponto`).
2. Coloque os 3 arquivos (`index.html`, `style.css`, `script.js`) na raiz do repositório.
3. Vá em **Settings > Pages**.
4. Em "Source", selecione a branch `main` (ou `master`) e a pasta `/ (root)`.
5. Salve. Em alguns minutos o app estará disponível em:
   `https://SEU-USUARIO.github.io/calculadora-ponto/`

