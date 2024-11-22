# Bitbucket Pipeline Example

Este projeto demonstra a configuração de um pipeline CI/CD usando o Bitbucket para realizar as seguintes etapas:

1. **Instalação de dependências**: Configura o ambiente Python e instala os pacotes necessários.
2. **Verificação de qualidade de código**: Usa o `flake8` para garantir o padrão de qualidade.
3. **Execução de testes unitários**: Utiliza o `unittest` para rodar os testes.
4. **Deploy automatizado**: Configura permissões e executa um script de deploy.
5. **Notificação no Slack**: Envia uma mensagem no Slack após o sucesso do pipeline.
6. **Steps manuais**: Inclui ações que podem ser disparadas manualmente, como notificações ou deploys adicionais.

---

## Como Usar Este Projeto

### 1. Pré-requisitos
Certifique-se de ter:
- Git instalado.
- Uma conta no GitHub e no Bitbucket.
- Webhook do Slack configurado (caso utilize o step de notificação).

### 2. Clone o Repositório
```bash
git clone https://github.com/thiagoaraujo2/bitbucket-pipeline-example.git
cd bitbucket-pipeline-example

### 3. Configuração do Pipeline
No arquivo bitbucket-pipelines.yml, configure os seguintes itens conforme necessário:

- Dependências no arquivo requirements.txt.
- Script de deploy (deploy.sh).
- Webhook do Slack no step de notificação.

## 4. Executando Localmente

Para testar o pipeline antes de rodar no Bitbucket:

1. Instale as dependências:
pip install -r requirements.txt

2. Rode os testes unitários:
python -m unittest discover

3. Verifique o estilo do código:
flake8 .

## 5. Deploy

Certifique-se de que o script deploy.sh está configurado e com permissões de execução:
 - chmod +x deploy.sh
 - ./deploy.sh

## Estrutura do Projeto

bitbucket-pipeline-example/
├── deploy.sh                # Script de deploy automatizado
├── requirements.txt         # Dependências do projeto
├── bitbucket-pipelines.yml  # Configuração do pipeline no Bitbucket
└── README.md                # Documentação do projeto

## Configuração do Bitbucket Pipeline

O pipeline é definido no arquivo bitbucket-pipelines.yml e contém os seguintes passos:

## Etapas Automáticas

- Instalar dependências: Instala os pacotes listados no requirements.txt.
- Verificação de qualidade de código: Usa o flake8 para garantir boas práticas.
- Testes unitários: Valida funcionalidades usando unittest.
- Deploy automatizado: Executa o script deploy.sh.

##Etapas Manuais

- Notificação no Slack: Dispara uma mensagem manualmente ao Slack.
- Deploy para Produção: Uma etapa manual para ambientes de produção.

## Contribuição

1. Faça um fork do repositório.

2. Crie uma branch para sua feature:
 - git checkout -b minha-feature

3. Commit suas mudanças:
 - git commit -m "Adiciona minha nova feature"

4. Envie sua branch:
 - git push origin minha-feature

5. Abra um Pull Request.

## Licença
Este projeto está licenciado sob a MIT License.

## Contato
Criado por Thiago de Araujo. Entre em contato para mais informações:

[LinkedIn](https://linkedin.com/in/jtabdesigner)
[GitHub](https://github.com/thiagoaraujo2)

### Instruções
- Substitua os links de contato com os seus reais.
- Edite o conteúdo conforme necessário para atender aos requisitos específicos do projeto.