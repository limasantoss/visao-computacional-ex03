# Atividade 03 - Filtragem de Imagens e Analise de Ruido

## 1. Objetivo

Este repositorio apresenta a Atividade 03 da disciplina de Visao Computacional. O foco do trabalho e observar como ruidos artificiais alteram imagens autorais e como filtros no dominio da frequencia podem ajudar na analise e no tratamento dessas degradacoes.

## 2. Imagens utilizadas

Foram utilizadas duas imagens autorais do dataset produzido anteriormente:

- `imagens/originais/sapato_01.jpg`
- `imagens/originais/skate_01.jpg`

## 3. Tecnicas aplicadas

O notebook aplica e discute:

- ruido gaussiano
- ruido sal e pimenta
- espectro de Fourier
- filtro passa-baixa gaussiano
- filtro passa-alta gaussiano
- comparacoes visuais
- tabela final de resultados
- conclusao critica

## 4. Estrutura de pastas

```text
visao-computacional-ex03/
|-- notebooks/
|   `-- atividade_03.ipynb
|-- imagens/
|   |-- originais/
|   |   |-- sapato_01.jpg
|   |   `-- skate_01.jpg
|   `-- processadas/
|-- docs/
|   `-- checklist_entrega.md
|-- README.md
`-- requirements.txt
```

## 5. Como executar

1. Criar o ambiente virtual com Python 3.12: `py -3.12 -m venv .venv`
2. Ativar o ambiente: `.\.venv\Scripts\Activate.ps1`
3. Instalar as dependencias: `pip install -r requirements.txt`
4. Abrir `notebooks/atividade_03.ipynb`
5. Selecionar o kernel `Python (visao-ex03)`
6. Rodar todas as celulas

## 6. Observacoes sobre os resultados

As imagens originais preservam melhor textura e bordas naturais. O ruido gaussiano espalha granulacao pela cena e o ruido sal e pimenta cria pontos extremos que afetam bastante a leitura visual. O espectro de Fourier ajuda a enxergar como a energia da imagem se organiza e como o ruido amplia componentes de alta frequencia. O filtro passa-baixa gaussiano reduz parte do ruido, mas suaviza contornos. O filtro passa-alta evidencia bordas e detalhes, porem tambem pode reforcar o proprio ruido.

## 7. Checklist rapido

- As imagens autorais estao em `imagens/originais`
- O notebook usa caminhos relativos
- Ha ruido gaussiano e sal e pimenta
- Ha espectro de Fourier das imagens originais e ruidosas
- Ha filtro passa-baixa gaussiano e filtro passa-alta
- Ha tabela final e conclusao critica
- O notebook deve ser executado por completo com o kernel `Python (visao-ex03)`
