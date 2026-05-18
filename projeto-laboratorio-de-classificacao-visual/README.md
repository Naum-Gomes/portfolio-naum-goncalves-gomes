# Laboratório de Classificação Visual: Calvo vs. Careca

Este repositório documenta um experimento de Visão Computacional realizado para o Laboratório de Engenharia de Software, explorando conceitos de treinamento de modelos, viés algorítmico e ética em Inteligência Artificial.

## 🎯 Objetivo do Projeto
O objetivo foi treinar um modelo de classificação de imagens capaz de distinguir entre duas categorias semelhantes ("Calvo" e "Careca") para observar como a qualidade e a diversidade dos dados de treinamento influenciam a precisão e o comportamento do algoritmo.

---

## 🛠️ Detalhes do Experimento

### 1. Conjunto de Dados (Dataset)
* **Classes:** Calvo e Careca.
* **Amostras:** Foram utilizadas 20 amostras de imagens para cada classe [cite: 541, 546].
* **Ferramenta:** Teachable Machine (Google) [cite: 561].

### 2. Resultados do Modelo
O modelo foi treinado com sucesso e testado com imagens reais para validação:
* **Teste Prático:** Em uma das validações, o modelo classificou corretamente uma imagem de teste com **100% de confiança** para a classe "Careca" [cite: 571].
* **Interface:** O sistema apresenta o output em tempo real, indicando a probabilidade para cada categoria mapeada [cite: 556].

---

## 🧠 Análise Crítica e Reflexão

### Mecanismo do Viés
Quando o conjunto de dados usado no treinamento é limitado, o algoritmo aprende apenas uma parte da realidade [cite: Screenshot_2.png]. A seleção restrita de imagens reduz a variedade de exemplos e faz o modelo associar certas características a uma categoria específica [cite: Screenshot_2.png]. Como resultado, o sistema baseia suas decisões em dados incompletos, criando uma visão distorcida da realidade [cite: Screenshot_2.png].

### Consequência Social
A classificação incorreta de pessoas pode gerar desconforto e frustração, diminuindo a confiança na tecnologia [cite: Screenshot_2.png]. Em contextos profissionais, erros desse tipo podem reforçar estereótipos ou reduzir oportunidades, impactando diretamente na percepção de justiça das pessoas [cite: Screenshot_2.png].

### Ação Mitigadora (Human-in-the-loop)
Para reduzir esse problema, é essencial incluir a participação humana no desenvolvimento [cite: Screenshot_2.png]. Especialistas devem revisar o conjunto de dados antes do treinamento para garantir diversidade [cite: Screenshot_2.png]. Durante os testes, avaliadores humanos identificam erros e padrões de viés, ajustando o conjunto de dados conforme necessário para um sistema mais justo [cite: Screenshot_2.png].

---

## 📁 Evidências do Projeto
* **Estrutura de Treinamento:** Visualização das classes e amostras carregadas [cite: evidencia.pdf].
* **Preview do Modelo:** Demonstração do output do modelo treinado [cite: ricardo.pdf].

---
**Desenvolvedor:** Naum Gonçalves Gomes  
**Data:** Abril de 2026
