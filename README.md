# Sistema-de-Busca-e-Resposta
Esse modelo é um sistema de busca e resposta inteligente que utiliza o poder do Google Generative AI. Ele analisa o significado das suas perguntas e encontra os documentos mais relevantes, mesmo que você não use as palavras-chave exatas. As respostas podem ser apresentadas de forma clara e concisa, facilitando a compreensão.


# Sistema de Busca e Resposta com Google Generative AI

Este projeto implementa um sistema de busca e resposta utilizando embeddings de texto e modelos de linguagem do Google Generative AI.

## Funcionalidades:
- Cria embeddings de texto para um conjunto de documentos.
- Realiza busca semântica para encontrar o documento mais relevante a uma consulta.
- Reescreve o conteúdo do documento selecionado em um estilo mais informal.

## Tecnologias:
**Google Generative AI:** 

    - `models/embedding-001` para gerar embeddings de texto.
    - `gemini-1.0-pro` para reescrever texto.

**Python:** Linguagem de programação principal.

**Pandas:** Biblioteca para manipulação e análise de dados.

**NumPy:** Biblioteca para computação numérica.

## Como funciona:

1. **Criação de Embeddings:** O código gera embeddings para um conjunto de documentos, capturando seu significado semântico.
2. **Busca Semântica:** Quando uma consulta é feita, ela é transformada em um embedding. O sistema compara o embedding da consulta com os embeddings de cada documento para encontrar o mais semelhante.
3. **Reescrita de Texto:** O conteúdo do documento selecionado pode ser reescrito de forma mais informal usando o modelo de linguagem `gemini-1.0-pro`.

## Como usar:

1. Clone o repositório.
2. Instale as bibliotecas necessárias: `pip install -U -q google-generativeai pandas numpy`.
3. Substitua `"YOUR_API_KEY"` no código pela sua chave de API do Google Generative AI.
4. Execute o código Python.


## Exemplo de uso:

                                consulta = "Como faço para trocar marchas em um carro do Google?"

                                 trecho = gerar_e_buscar_consulta(consulta, df, model)
                                 print(trecho)

                                # ... (reescrita do texto)



## Observações:

- O modelo `gemini-1.0-pro` pode estar sujeito a custos de uso.
- A qualidade da resposta depende da qualidade dos dados e da capacidade dos modelos.

## Possíveis Aplicações:

- Chatbots
- Sistemas de perguntas e respostas
- Recuperação de informações
- Sumarização de texto
- Geração de conteúdo


## Contribuições:

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.
