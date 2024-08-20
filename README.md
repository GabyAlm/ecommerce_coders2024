# Sistema de Gerenciamento de Vendas e Inventário

## Objetivo

O objetivo deste projeto é desenvolver um sistema robusto e eficiente de gerenciamento de inventário para uma loja virtual. O sistema permite o cadastro, atualização, exclusão e listagem de produtos, além de realizar vendas e gerar relatórios detalhados em formato TXT. Foi projetado para lidar com erros na inserção de dados e oferecer uma interface amigável para os usuários.

## Funcionalidades

### 1. Cadastro de Produtos
**Informações do Produto**: Nome, categoria, preço, quantidade em estoque e descrição opcional.
**Armazenamento**: Produtos são armazenados utilizando dicionários indexados por um identificador único.

### 2. Atualização de Produtos
**Atualizações Possíveis**: Nome, chave, preço, quantidade em estoque e descrição.
**Validação**: Mecanismos de validação para evitar erros comuns.

### 3. Exclusão de Produtos
**Remoção Segura**: Exclusão de produtos do inventário via chave de identificação única com tratamento de exceções para produtos inexistentes.

### 4. Realização de Vendas
**Atualização de Estoque**: Estoque atualizado automaticamente após cada venda.
**Tratamento de Exceções**: Verificação de estoque insuficiente com mensagens de erro claras.

### 5. Relatórios de Vendas
**Formato TXT**: Geração de relatórios em formato TXT contendo informações detalhadas da venda.
**Informações Solicitadas**: Chave do produto, quantidade vendida.

### 6. Persistência de Dados
**Arquivos de Dados**: Dados do inventário e informações de vendas são persistidos em arquivos de texto, garantindo a persistência entre execuções.

### 7. Tratamento de Exceções
**Exceções Personalizadas**: Tratamento robusto de exceções para cadastro, atualização e exclusão.
**Erros de Estoque**: Exceções personalizadas para erros de estoque insuficiente e manipulação inadequada de dados.

### 8. Interface com o Usuário
**Interação Amigável**: Menus e opções claras que guiam o usuário durante o uso do sistema.
**Flexibilidade**: Uso de funções com parâmetros variáveis para maior flexibilidade.

### 9. Técnicas Funcionais
**Programação Funcional**: Uso de funções lambda para manipulação e processamento eficiente de listas de produtos e vendas.

### 10. Documentação
**Documentação Completa**: Descrição da arquitetura e exemplos de uso para facilitar o entendimento dos usuários.

## Estrutura do Projeto

├── data/
│   ├── estoque_de_produtos.txt
│   └── Relatório_de_vendas.txt
├── src/
│   ├── system.py
├── venv/
├── README.md
└── requirements.txt

## Uso

**Configuração do Ambiente**

git clone https://github.com/ju4nv1e1r4/ecommerce_coders2024.git
cd diretorio/do/projeto
python3 -m venv venv
source venv/bin/activate 
pip install -r requirements.txt
