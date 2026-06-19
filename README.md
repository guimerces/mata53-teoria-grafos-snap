# TP: Analisando Grafos do SNAP - Epinions

Repositório contendo os códigos e análises para o Trabalho Prático da disciplina de Teoria dos Grafos.

**Autor:** Guilherme Antonio Merces Silva (Matrícula: 223118823)  
**Dataset Base:** [Epinions Social Network (SNAP)](http://snap.stanford.edu/data/soc-sign-epinions.html)

---

## Tecnologias Utilizadas
Este projeto foi desenvolvido utilizando as seguintes tecnologias:
- **Python 3.10+** (Linguagem base)
- **Jupyter Notebook** (Ambiente de execução e relatório interativo)
- **NetworkX** (Extração de métricas, busca de caminhos mínimos e algoritmos de grafos estruturais)
- **Matplotlib** (Visualização gráfica da Lei de Potência e Distribuição de Graus)
- **NumPy & SciPy** (Cálculos matemáticos, médias e intervalos de confiança estatística)

## Estrutura do Projeto
- `TP_Grafos_Epinions.ipynb`: O Jupyter Notebook principal contendo todo o código executável, dividido didaticamente nas três partes do trabalho (Análise Estrutural, Algoritmos e Propriedades Avançadas).
- `soc-sign-epinions.txt`: O arquivo de dados original da rede social, já preparado e pronto para uso.
- `requirements.txt`: Lista exata de dependências para reprodutibilidade.

## Como Executar (Reprodutibilidade)

Para garantir que a simulação rode perfeitamente no seu computador local, siga os passos abaixo:

### 1. Preparando o Ambiente
Recomenda-se fortemente a utilização de um ambiente virtual para não gerar conflitos de versões.
Abra o terminal na pasta do projeto e execute:

```bash
# Criar ambiente virtual
python -m venv .venv

# Ativar ambiente virtual (Windows)
.venv\Scripts\activate
# Ativar ambiente virtual (Linux/Mac)
source .venv/bin/activate
```

### 2. Instalando as Dependências
Com o ambiente ativado, instale as bibliotecas utilizadas no projeto:
```bash
pip install -r requirements.txt
```

### 3. Rodando as Análises
Você pode abrir e rodar o arquivo de duas formas:
- **Opção A (Navegador):** No terminal, digite `jupyter notebook`. O arquivo `TP_Grafos_Epinions.ipynb` abrirá no seu navegador. Basta rodar as células em sequência.
- **Opção B (VS Code):** Abra o arquivo `TP_Grafos_Epinions.ipynb` no VS Code, certifique-se de escolher o ambiente `.venv` que você acabou de criar clicando em "Select Kernel" no canto superior direito, e rode as células.

> **Nota de Performance:** Devido ao tamanho do grafo original (130 mil vértices e 840 mil arestas), algoritmos com complexidade O(V*E) ou superior (como o cálculo exato do diâmetro e clusterização em rede total) podem demorar um longo tempo. Os valores originais já catalogados pela Stanford University foram citados no relatório para estas métricas em específico.