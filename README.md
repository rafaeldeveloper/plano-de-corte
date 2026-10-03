# Plano de Corte

Otimizador de corte de chapas (MDF, MDP, compensado, aço, vidro) a partir de um arquivo de medidas. Roda inteiro no navegador, sem servidor.

**Acesse:** https://rafaeldeveloper.github.io/plano-de-corte/

## Como usar

1. Escolha a chapa (ou informe medidas próprias), a espessura da serra e o refilo.
2. Importe o arquivo de medidas (`.xlsx`, `.xls`, `.ods`, `.csv`, `.txt`) ou cole da planilha.
3. Veja o desenho de cada chapa, o aproveitamento, a sequência de cortes e os retalhos.
4. Copie o plano em CSV.

## Formato do arquivo

Colunas reconhecidas pelo cabeçalho: `Peça`, `Comprimento`, `Largura`, `Quantidade`, `Girar` ou `Veio`. Sem cabeçalho, a ordem usada é nome, comprimento, largura, quantidade. Medidas em mm; cabeçalho com `(cm)` ou `(m)` é convertido. Veja `exemplo_medidas.csv`.

## Modos

- **Guilhotina**: cortes de ponta a ponta (esquadrejadeira, seccionadora). Gera a sequência numerada de cortes.
- **Livre**: encaixe sem restrição de guilhotina (CNC, laser).
