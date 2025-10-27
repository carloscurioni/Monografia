# Monografia

Este repositório contém a fonte LaTeX e o código Python associados usados para produzir o artigo acadêmico.

Estrutura
- paper/: fontes LaTeX, bibliografia e figuras
- src/: scripts e módulos Python usados para análise e geração de figuras
- notebooks/: notebooks exploratórios (Jupyter ou convertidos para Markdown)
- .github/workflows/: CI para compilar o PDF

Como compilar (local)
1. (Recomendado) Crie um ambiente virtual:
   ```sh
   python -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```
2. Compile o PDF (é necessário latexmk):
   ```sh
   make pdf
   ```
   ou
   ```sh
   ./build.sh
   ```

Notas
- A compilação LaTeX usa `latexmk` e pode requerer `-shell-escape` se o pacote minted for usado.
- Adicione figuras em `paper/figures/` e referencie-as nas seções.
- A bibliografia está em `paper/references.bib`.

Licença: adicione sua licença preferida em LICENSE.