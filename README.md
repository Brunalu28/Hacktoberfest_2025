# 🤖 Construindo Agentes Inteligentes com Plataformas Open Source

## Apresentação

Este repositório contém todo o material prático e os notebooks Jupyter utilizados no workshop **"Construindo agentes inteligentes utilizando plataformas Open Source"**.

O objetivo deste material é demonstrar, de forma prática e acessível, como prototipar e desenvolver sistemas de Agentes Inteligentes utilizando ferramentas e bibliotecas abertas, com foco especial em modelos de linguagem (LLMs) executados localmente.

## 📚 Conteúdo do Repositório

O repositório é composto por dois notebooks principais que demonstram a construção de agentes com diferentes fontes de dados e técnicas de pré-processamento:

| Notebook                                    | Descrição                                                                                                                                                                                                                           | Principais Tópicos Abordados                                                                                                                         |
| :------------------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`Agentes_inteligentes_texto_fixo.ipynb`** | Demonstra a criação de agentes que processam **texto estático** (strings ou listas de texto) para realizar tarefas como resumo, extração de conceitos-chave e geração de perguntas de estudo.                                       | Prompt Engineering, Cadeias (Chains) da LangChain, LLM de código aberto.                                                                             |
| **`Agentes_inteligentes_pdf.ipynb`**        | Foca na criação de agentes para processamento de dados de **documentos não estruturados (PDFs)**. Demonstra a extração de texto de todas as páginas do documento, sua concatenação e pré-processamento para posterior envio ao LLM. | Carga de PDFs, Extração e Concatenação de Texto, Processamento Direto de Documentos Inteiros com LLMs (considerando o limite de contexto do modelo). |

## 🚀 Tecnologias Utilizadas

As seguintes ferramentas e bibliotecas open source são a base deste workshop:

- **Python:** Linguagem de programação principal.
- **LangChain:** Framework essencial para orquestração de componentes de LLMs (Chains, Prompts, Agentes).
- **`llama-cpp-python`:** Biblioteca para execução de modelos LLM em formato GGUF (quantizado) de forma eficiente.
- **Modelos Open Source (GGUF):** Modelos de linguagem de código aberto que podem ser executados localmente (e.g., Llama, Mistral).
- **Outras bibliotecas:** `pypdf` (para leitura de PDFs).

## 💻 Como Executar os Notebooks

Para replicar o ambiente do workshop e executar os notebooks em sua máquina, siga os passos abaixo:

### Pré-requisitos

1.  **Python 3.8+** instalado.
2.  **Jupyter Notebook** ou **JupyterLab** instalado (ou use um ambiente como Google Colab).

### Configuração do Ambiente

1.  **Clone o repositório:**

    ```bash
    git clone <URL_DO_SEU_REPOSITORIO>
    cd <NOME_DO_REPOSITORIO>
    ```

2.  **Crie um ambiente virtual (Recomendado):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # No Linux/macOS
    # .\venv\Scripts\activate # No Windows
    ```

3.  **Instale as dependências:**
    Ambos os notebooks contêm comandos `!pip install -qU ...` nas primeiras células para garantir que todas as dependências (LangChain, llama-cpp-python, pypdf, etc.) sejam instaladas corretamente.

4.  **Execute o Jupyter:**
    ```bash
    jupyter notebook
    ```
    Ou abra os arquivos `.ipynb` diretamente no seu ambiente de desenvolvimento.

### 📝 Observação Importante sobre o LLM

Os notebooks estão configurados para usar um **LLM de código aberto** via `llama-cpp-python`. Isso geralmente requer o download de um arquivo de modelo (e.g., um arquivo `.gguf`).

- Recomendo o uso do **Google Colab** para facilitar a execução, pois ele pode lidar com a instalação de bibliotecas e o uso de GPUs de forma mais simples.

## 🤝 Contribuição

Contribuições são bem-vindas! Se você encontrou um erro, tem uma sugestão de melhoria ou deseja adicionar um novo exemplo, sinta-se à vontade para abrir uma _Issue_ ou enviar um _Pull Request_.
