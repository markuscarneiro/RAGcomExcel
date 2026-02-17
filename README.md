# Análise Financeira com RAG em Excel e IA Generativa

Este projeto é uma aplicação de RAG (Geração Aumentada por Recuperação) projetada para realizar análises financeiras inteligentes em planilhas Excel utilizando IA Generativa local. Construído com Streamlit, LlamaIndex e Ollama.

A aplicação permite que os usuários façam upload de planilhas financeiras e façam perguntas complexas sobre os dados, aproveitando o poder de LLMs locais para fornecer respostas contextualizadas, mantendo a privacidade dos dados.

## 🚀 Funcionalidades

- **Integração com Excel**: Upload e processamento simples de arquivos `.xlsx` e `.xls`.
- **Visualização Interativa de Dados**: Visualize os dados da sua planilha diretamente na interface do aplicativo.
- **Análise Impulsionada por IA**: Faça perguntas em linguagem natural sobre seus dados financeiros.
- **Privacidade Local**: Utiliza LLMs locais (Llama 3.2 via Ollama), garantindo que dados financeiros sensíveis nunca saiam da sua máquina.
- **Consciência de Contexto**: Recupera informações relevantes da planilha para responder a consultas específicas.
- **Gerenciamento de Sessão**: Mantém o histórico de chat e armazena em cache arquivos processados para eficiência.

## 🛠️ Tecnologias Utilizadas

- **Python 3.12+**
- **[Streamlit](https://streamlit.io/)**: Interface web interativa.
- **[LlamaIndex](https://www.llamaindex.ai/)**: Framework para conectar fontes de dados personalizadas a LLMs.
- **[Ollama](https://ollama.com/)**: Executor de LLM local.
- **HuggingFace Embeddings**: Modelo `BAAI/bge-large-en-v1.5` para busca semântica.
- **Docling**: Análise avançada de documentos.
- **Pandas**: Manipulação e análise de dados.

## 📋 Pré-requisitos

Antes de executar a aplicação, certifique-se de ter o seguinte instalado:

1. **Python**: Python 3.12 ou superior é recomendado.
2. **Ollama**: Baixe e instale o Ollama em [ollama.com](https://ollama.com/).
3. **Modelo Llama 3.2**: Baixe o modelo necessário usando a linha de comando:
   ```bash
   ollama pull llama3.2
   ```

## 📦 Instalação

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/seu-usuario/financial-rag-excel.git
   cd financial-rag-excel
   ```

2. **Configure um Ambiente Virtual**:

   **Usando `venv`**:
   ```bash
   python -m venv venv
   # Windows
   .\venv\Scripts\activate
   # Linux/Mac
   source venv/bin/activate
   ```

   **Usando `conda`** (alternativa):
   ```bash
   conda create --name rag-excel python=3.12
   conda activate rag-excel
   ```

3. **Instale as Dependências**:
   ```bash
   pip install -r requirements.txt
   ```

## ▶️ Como Usar

1. **Execute a Aplicação Streamlit**:
   ```bash
   streamlit run app.py
   ```

2. **Acesse a Aplicação**:
   Abra seu navegador e navegue até a URL local fornecida (geralmente `http://localhost:8501`).

3. **Instruções de Uso**:
   - **Upload**: Use a barra lateral para fazer upload do seu arquivo Excel financeiro.
   - **Indexação**: Aguarde o sistema indexar o documento (uma mensagem de sucesso "Sistema Pronto!" aparecerá).
   - **Pergunte**: Digite sua pergunta na entrada de chat, por exemplo, "Qual foi a receita total no 1º trimestre?" ou "Compare as despesas entre janeiro e fevereiro".
   - **Limpar**: Use o botão "Limpar" para apagar o histórico de chat e iniciar uma nova sessão de análise.

## 🧩 Estrutura do Projeto

```
├── app.py              # Código principal da aplicação
├── requirements.txt    # Dependências Python
├── README.md           # Documentação do projeto
```

## 🤝 Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para enviar um Pull Request.

1. Faça um Fork do projeto
2. Crie sua branch de feature (`git checkout -b feature/RecursoIncrivel`)
3. Faça o Commit das suas alterações (`git commit -m 'Adiciona algum RecursoIncrivel'`)
4. Faça o Push para a branch (`git push origin feature/RecursoIncrivel`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
