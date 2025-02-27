# Evolution API - Setup com aaPanel e Docker Compose

Este repositório contém instruções para configurar e executar a Evolution API utilizando o aaPanel e Docker Compose.

## Pré-requisitos
- **aaPanel** instalado
- **Docker** e **Docker Compose** instalados no aaPanel
- **Acesso** ao painel do aaPanel

## Passo a Passo

### 1. Criar Template do Compose no aaPanel
1. Acesse o seguinte caminho no aaPanel:
   ```
   Docker -> Compose -> Template List
   ```
2. Crie um novo template com o nome **evolution-api-template**.
3. Cole o conteúdo do arquivo `compose.yaml` no template.
4. **Atenção:** Pode ocorrer um problema onde o arquivo `.env` não é localizado. Caso isso aconteça, remova a linha correspondente e adicione novamente após a criação do template.

### 2. Criar um Novo Compose
1. Acesse o seguinte caminho no aaPanel:
   ```
   Docker -> Compose -> Add Compose
   ```
2. Selecione o template criado anteriormente (**evolution-api-template**).
3. No campo `.env` do compose, cole o conteúdo do arquivo `.env`.
4. Aguarde a finalização do deployment.

## 📚 Documentação
Para mais detalhes, consulte a documentação oficial:
- [📖 Instalação via Docker](https://doc.evolution-api.com/v2/pt/install/docker)
- [⚙️ Variáveis de Ambiente](https://doc.evolution-api.com/v2/pt/env)

