# Aplicação de Perguntas e Respostas sobre os padrões operacionais da companhia utilizando BERT (Pre-Training of Deep Biredictional Transformers For Language Understanding)

#### Aluno: [André Roberto Antunes Paes](https://github.com/arobertoap).
#### Orientador: [Leonardo Alfredo Forero Mendoza](https://github.com/leofome8).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- [Link para o arquivo Readme](https://github.com/arobertoap/TCC_BI_Master_Publico)
- [Link para o código](https://github.com/arobertoap/TCC_BI_Master) (o repositório é privado e só pode ser acessado com a autorização do autor).

- Trabalhos relacionados: <!-- caso não aplicável, remover estas linhas -->
    - [Jacob Devlin   Ming-Wei Chang   Kenton Lee   Kristina Toutanova - BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805)
    - [NeuralMind - Modelos BERT em português](https://github.com/neuralmind-ai/portuguese-bert)
    - [DeepLearning Brasil - SQuAD em português](https://drive.google.com/file/d/1Q0IaIlv2h2BC468MwUFmUST0EyN7gNkn/view?usp=sharing)
    - [Hugging Face - Biblioteca Transformer](https://huggingface.co/transformers/)


---

### Resumo

A solução de chatbot atualmente utilizada pela organização requer que, previamente, sejam cadastrados pares de perguntas/respostas para que, dada uma questão colocada por usuário, seja possível prover a resposta mais provável com bases nesses pares. Para o caso dos padrões de operação (descrição pormenorizada dos procedimentos operacionais), isso requer uma constante manutenção na atualização dos pares e a impossibilidade da solução responder a perguntas que não tenham sido previstas.

O objetivo do trabalho foi o de criar um modelo que "aprendesse" com próprios textos dos padrões e “gerasse” a resposta a partir dos mesmos. Para tanto, foram utilizados como bases um modelo BERT (PRE-TRAINING OF DEEP BIDIRECTIONAL TRANSFORMERS FOR LANGUAGE UNDERSTANDING) treinado em português e um dataset com cerca de 87.000 perguntas e respostas anotadas (SQuAD - Stanford Question Answering Dataset) também em português.

Ao contrário de outros modelos de representação de linguagem, BERT é projetado para pré-treinar representações bidirecionais profundas de textos não rotulados, condicionando conjuntamente o contexto esquerdo e direito em todas as camadas. Como resultado, o modelo BERT pré-treinado pode ser ajustado com apenas uma camada de saída adicional para criar modelos de última geração para uma ampla gama de tarefas, tais como perguntas & respostas e inferência de linguagem, sem substanciais modificações específicas na sua arquitetura [[
arXiv:1810.04805]](https://arxiv.org/abs/1810.04805).

Os resultados, ou seja, as respostas dadas às perguntas feitas sobre os padrões, foram impressionantemente corretos. Medindo os resultados de forma mais precisa, o modelo obteve 72% de acurácia em uma parte do conjunto de dados SQuAd reservada para teste, ou seja, gerou exatamente a resposta esperada nesses casos. Para aquelas que não eram exatas, a distância do erro mediano, ou seja, a diferença mediana entre o caracter onde começou a resposta real e gerada, foi de 28 posições. 

### Abstract 

The current chatbot solution used by the organization requires that, previously, pairs of questions/answers are registered. Thus, given a question posed by the user, it is possible to provide the most likely answer based on the pairs. In the case of operating standards (detailed description of operating procedures), this requires a constant maintenance of pair updates and the inability of the solution to answer questions that have not been foreseen.

The objective of the work was to create a model that "learn" from the standards texts themselves and "generate" the answer from them. Therefore, a BERT model (PRE-TRAINING OF DEEP BIDIRECTIONAL TRANSFORMERS FOR LANGUAGE UNDERSTANDING) trained in Portuguese and a dataset with about 87,000 annotated questions and answers (SQuAD - Stanford Questioning Dataset) also in Portuguese were used as bases.

Unlike other language representation models, BERT is designed to pre-train deep bidirectional representations from unlabeled text by jointly conditioning on both left and right context in all layers. As a result, the pre-trained BERT model can be fine-tuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial task-specific architecture modifications [[
arXiv:1810.04805]](https://arxiv.org/abs/1810.04805).

The results, that is, the answers given to the questions asked about the standards, were impressively correct. Measuring the results more precisely, the model obtained 72% accuracy in a portion of the SQuAd dataset reserved for testing, that is, it generated the exactly expected response in these cases. For those that were not exact, the median error distance, that is, the median difference between the character where the real and generated response began, was 28 positions. 

---

Matrícula: 192.671.013

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
