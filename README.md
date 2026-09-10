# 🚀 Projeto Prático: DevOps e Integração Contínua (UNINTER)

![CI Docker Pipeline](https://github.com/ewaldohenrique3/trabalho_devops_uninter/actions/workflows/pipeline.yml/badge.svg)

## 🎯 Sobre o Projeto
Esta aplicação web foi desenvolvida como atividade prática para a disciplina de **DevOps e Integração Contínua** do Centro Universitário Internacional UNINTER.

O projeto simula a atuação de uma consultoria de DevOps contratada para reestruturar os processos de desenvolvimento da empresa fictícia **CodeFactory Solutions**. A proposta é demonstrar, na prática, como a adoção da cultura DevOps — por meio do versionamento estruturado, automação de testes e containerização — soluciona problemas de atrasos, falta de padronização e dificuldades na integração de software.

---

## 💻 A Aplicação
A plataforma consiste em um portal informativo construído em HTML5 e CSS3, apresentando a estrutura da equipe de consultoria, documentação técnica das etapas do fluxo DevOps e métricas do ambiente de desenvolvimento.

---

## 🧰 Práticas e Tecnologias Aplicadas
* **Git & GitHub:** Versionamento de código, controle de fluxo por branches, gestão de histórico de commits e resolução de conflitos.
* **Gestão & Colaboração:** Utilização de Issues, Projects, Labels, Milestones e Wiki do GitHub para acompanhamento do ciclo de vida da aplicação.
* **Docker & Nginx:** Containerização do ambiente web utilizando servidor Nginx (imagem leve `alpine`), garantindo portabilidade e padronização da aplicação.
* **Integração Contínua (CI):** Pipeline automatizada via GitHub Actions para validação de arquivos estáticos, testes de build da imagem Docker e verificação de saúde (*health check*) do container.

---

## 👥 Equipe de Desenvolvimento

| Integrante | RU (Registro Unificado) |
| :--- | :--- |
| Hallyson Lucas de Moura Lima | 5212947 |
| Ewaldo Henrique Soares de Moura | 5212858 |
| Gabriel Almeida Cardillo | 5223842 |

---

## ⚙️ Como Executar o Projeto Localmente com Docker

Se você quiser subir o container do site na sua máquina para testes, siga os passos abaixo:

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/ewaldohenrique3/trabalho_devops_uninter.git](https://github.com/ewaldohenrique3/trabalho_devops_uninter.git)
   cd trabalho_devops_uninter