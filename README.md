# Projeto: Fine-tuning GPT-2 em Sintomas de Doenças

Este projeto realiza o **treinamento de um modelo de linguagem (GPT-2)** utilizando um dataset de sintomas de doenças, com foco em gerar texto coerente a partir de combinações entre nome da doença e seus sintomas.

## 🚀 Funcionalidades

* Download do dataset [Diseases\_Symptoms](https://huggingface.co/datasets/QuyenAnhDE/Diseases_Symptoms) do Hugging Face.
* Pré-processamento dos dados em **Pandas**.
* Criação de dataset customizado compatível com **PyTorch**.
* Fine-tuning do modelo **DistilGPT-2**.
* Monitoramento de métricas de treino e validação.
* Geração de texto a partir do modelo ajustado.
* Tradução automática para português utilizando `googletrans`.

## 🛠️ Tecnologias Utilizadas

* [Python 3](https://www.python.org/)
* [PyTorch](https://pytorch.org/)
* [Transformers (Hugging Face)](https://huggingface.co/transformers/)
* [TorchText](https://pytorch.org/text/)
* [Pandas](https://pandas.pydata.org/)
* [Datasets (Hugging Face)](https://huggingface.co/docs/datasets)
* [TQDM](https://tqdm.github.io/)
* [Googletrans](https://pypi.org/project/googletrans/)

## 📂 Estrutura do Projeto

```
├── slm.py              # Script principal (extraído do notebook)
├── README.md           # Documentação do projeto
```

## ⚙️ Como Executar

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

### 2. Instalar dependências

```bash
pip install torch torchtext transformers sentencepiece pandas tqdm datasets googletrans==4.0.0-rc1
```

### 3. Executar o script

```bash
python slm.py
```

## 📊 Resultados Esperados

Durante o treinamento:

* Perdas de treino e validação são exibidas com **TQDM**.
* Métricas são salvas em um **DataFrame Pandas**.

Na geração de texto:

* O modelo gera texto baseado em sintomas e doenças.
* O resultado pode ser traduzido automaticamente para português.

## 📌 Status do Projeto

Este repositório foi utilizado como **material de estudo e prática** para reunir informações e treinar conceitos de **SLM (Small Language Models)** e **fine-tuning** aplicados a dados médicos, no contexto do meu projeto **PIBIC**.

## 🔮 Próximos Passos

* Salvar checkpoints do modelo.
* Avaliar perplexidade e métricas adicionais.
* Expandir para datasets médicos mais robustos.
* Criar API para consulta em tempo real.

---

✍️ Desenvolvido no contexto de estudos em **Processamento de Linguagem Natural (PLN)** e **IA aplicada à saúde**.
