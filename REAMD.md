# Alouvre - Sistema Gerenciador de Fotos, Imagens e Vídeos

**Versão**: 2.0  
**Autor**: Jorge Miguel Aviles de Moura  
**Data**: 09/2024

## Objetivo

Atualizar o sistema antigo do Alouvre, que é um gerenciador de fotos, imagens e vídeos, proporcionando aos usuários a capacidade de rastrear esses arquivos de forma mais rápida e intuitiva possível.

---

## Funcionalidades Principais

### Modo Normal

- **Projeto**: Usuários têm acesso à visualização e ao download dos arquivos.

### Modo Gerente

- **Gerenciamento de Pastas**: Capacidade de gerenciar totalmente as pastas, onde os arquivos serão armazenados.
- **Gerenciamento de Arquivos**: Permite editar e visualizar informações adicionais para facilitar a localização.
- **Peculiaridades**: Banco de dados com características personalizadas exclusivas de cada arquivo.
- **Filtros**: Filtros avançados para facilitar a edição e download de arquivos e pastas.

---

## Especificações de Funcionalidades

1. **Projeto**
2. **Gerenciamento de Especificidade**
3. **Gerenciamento de Arquivos**
4. **Gerenciamento de Pastas**

---

## Requisitos para Desenvolvimento

### Softwares Necessários

1. Servidor WEB
2. Servidor de Banco de Dados MySQL
3. Linguagem de Programação JavaScript
4. Linguagem de Programação PHP
5. Editor de Código (IDE) como Visual Studio
6. SGDB Workbench
7. Unix

### Outras Tecnologias

- **Bootstrap**
- **jQuery**
- **React**
- **Django**

---

## Arquitetura e Diagrama de Blocos

### Banco de Dados

O banco de dados do Alouvre será composto por 3 tabelas iniciais e outras tabelas criadas para particularidades dos arquivos.

#### Tabelas Principais

- **table_files**  
  Campos: `id`, `name`, `name_from_customer`, `code_digitable`, `material`, `localization`, `date`, `branch_of_activity`

- **table_folder**  
  Campos: `id`, `id_files`, `name`, `name_from_customer`, `code_digitable`, `material`, `localization`, `date`, `branch_of_activity`, `case`, `particularity_from_files`

- **table_particularity**  
  Campos: `id`, `keys_description`, `values_descriptions`

---

## Segurança

O serviço de segurança será baseado na integração com o microserviço de gerenciamento de usuários do sistema **Control Access**. Isso garantirá que apenas usuários autorizados possam acessar e gerenciar os arquivos e pastas.

---

## Implantação e Suporte

### Implantação

- O sistema será instalado no servidor central em nuvem da empresa, utilizando a porta `10.0.0.184` como ponto de acesso.
- O banco de dados MySQL será acessado via **PuTTY**.
- O **GitHub** será utilizado para a transferência de arquivos de código (.py e .js) para o ambiente de nuvem de forma segura.

### Configurações do Ambiente

- O acesso ao sistema será feito a partir de um PC da equipe de TI, que possui acesso direto à nuvem via **WinSCP**.
- Será necessário criar um novo banco de dados no **MySQL**, com um usuário dedicado para o sistema.

### Testes e Verificação

- O sistema será testado de acordo com a metodologia ágil adotada pela empresa. Após a implementação de cada funcionalidade, a equipe de Controle de Qualidade (QA) avaliará e aprovará cada etapa antes de prosseguir.

### Suporte Pós-Implantação

- Haverá suporte contínuo da equipe de desenvolvimento web para corrigir possíveis bugs e manter a funcionalidade do sistema.
- O suporte será focado em questões técnicas e funcionais que possam afetar o desempenho e a usabilidade do sistema.

---

## Treinamento e Documentação

- As equipes atuais já estão capacitadas para usar o software. No caso de novos usuários, o treinamento será feito por meio do compartilhamento de conhecimentos entre os próprios usuários.
- A documentação completa do sistema estará disponível no departamento de TI, fornecendo informações detalhadas sobre o uso e as funcionalidades do sistema.

---

## Introdução às Funcionalidades

### Modo Normal

- **Projeto**: Usuários poderão visualizar e fazer o download dos arquivos de forma geral.

### Modo Gerente

- **Gerenciamento de Pastas**: Capacidade de gerenciar todas as pastas e arquivos.
- **Arquivos**: Visualização avançada com textos descritivos para ajudar na localização dos arquivos.
- **Peculiaridades**: Banco de dados customizado com características únicas para cada arquivo.
- **Filtros**: Ferramentas para editar e baixar arquivos de forma rápida e eficiente.

---

## Coleta de Dados e Filtragem

### Coleta de Dados

A interface de front-end coleta os dados necessários para análise. Os usuários inserem especificações técnicas e outros dados relevantes para gerenciar as imagens.

### Filtragem de Dados

Após a coleta, os dados são filtrados para facilitar a localização de arquivos específicos, acelerando o processo de rastreamento de imagens pela equipe de marketing.

---
### Link figma
https://www.figma.com/design/IsDks8Y629OlajBaV8YqHd/Untitled?node-id=0-1&t=jiR8uQORfJateB3A-1

---

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests no repositório do projeto no GitHub.

---

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](./LICENSE) para obter mais detalhes.