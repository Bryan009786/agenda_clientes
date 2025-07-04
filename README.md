# 🧾 Gerenciador de Clientes - Documentação para Iniciantes

Bem-vindo ao **Gerenciador de Clientes**, uma aplicação simples em **Python** que ajuda a gerenciar informações de clientes (como nome, sobrenome, email e CPF) usando um banco de dados **SQLite**.

Este projeto é ideal para alunos que estão começando a aprender **Python**, **SQL**, **SQLite** e **Tkinter**, oferecendo um ótimo exemplo de aplicação CRUD com interface gráfica.

---

## 🧩 O que esta aplicação faz?

A aplicação permite:

- ✅ **Adicionar** novos clientes ao banco de dados
- 📋 **Visualizar** todos os clientes cadastrados
- 🔍 **Buscar** clientes por nome, sobrenome, email ou CPF
- ✏️ **Atualizar** dados de um cliente existente
- 🗑️ **Deletar** clientes do banco

A interface gráfica, criada com Tkinter, é simples e intuitiva. Os dados são armazenados em um arquivo local chamado `clientes.db`.

---

## 📁 Estrutura do Projeto

O projeto é organizado em **três arquivos principais**:

### `Gui.py`
- Cria a interface gráfica com Tkinter.
- Campos de texto, botões de ação (Adicionar, Atualizar, Deletar, Buscar, Limpar) e tabela com os dados dos clientes.
- Interage com o backend para executar as operações no banco.

### `Backend.py`
- Gerencia a conexão e as operações com o banco de dados SQLite.
- Contém métodos como:
  - `insert()`
  - `view()`
  - `search()`
  - `update()`
  - `delete()`
- Utiliza SQL parametrizado para evitar injeções.

### `application.py`
- Arquivo principal da aplicação.
- Inicializa o banco de dados e a interface.
- Contém a função `main()` que executa o sistema.

---

## 🛠️ Pré-requisitos

Você precisará de:

- ✔️ Python 3.8 ou superior  
  [Download oficial](https://www.python.org/downloads/)
- ✔️ Tkinter (incluso com Python)
- ✔️ SQLite (incluso no Python via `sqlite3`)
- ➕ **PyInstaller** (opcional) para gerar um executável `.exe`

---

## 🚀 Como Configurar e Executar

### 1. Criar a pasta do projeto

```bash
mkdir gerenciador_clientes
cd gerenciador_clientes
Salve os três arquivos Gui.py, Backend.py, application.py dentro desta pasta.

2. Verifique se o Python está instalado
bash
Copiar
Editar
python --version
Se não estiver, instale o Python.

3. Execute a aplicação
bash
Copiar
Editar
python application.py
Uma janela gráfica será exibida com a interface da aplicação.

🧑‍💻 Como Usar a Aplicação
A janela da aplicação inclui:

Campos de entrada: Nome, Sobrenome, Email, CPF

Botões de ação:

➕ Adicionar

📝 Atualizar

❌ Deletar

🔍 Buscar

🧹 Limpar

Tabela Treeview: Lista todos os clientes

▶️ Etapas Comuns
✅ Adicionar cliente
Preencha os campos

Clique em "Adicionar"

A tabela será atualizada automaticamente

🔍 Buscar cliente
Digite nome, email, CPF ou sobrenome

Clique em "Buscar"

Resultados filtrados serão mostrados

📝 Atualizar cliente
Clique em um cliente na tabela

Edite os campos

Clique em "Atualizar"

❌ Deletar cliente
Selecione o cliente na tabela

Clique em "Deletar"

🧹 Limpar campos
Clicando em "Limpar", todos os campos são apagados

📦 Criando um Executável com PyInstaller
1. Instalar o PyInstaller
bash
Copiar
Editar
pip install pyinstaller
2. Criar o executável
bash
Copiar
Editar
pyinstaller --onefile --noconsole application.py
O executável será gerado dentro da pasta /dist

3. Rodar o executável
bash
Copiar
Editar
cd dist
./application.exe
💡 Dica
Compartilhe apenas o .exe e o clientes.db (se quiser manter os dados)

O .exe pode ter entre 50-100MB por incluir todas as dependências

🗃️ Estrutura do Banco de Dados
Arquivo: clientes.db
Tabela: clientes

Campo	Tipo	Descrição
id	INT	Chave primária, auto-incremento
nome	TEXT	Nome do cliente
sobrenome	TEXT	Sobrenome do cliente
email	TEXT	Email do cliente
cpf	TEXT	CPF do cliente (com zeros à esquerda)

🧰 Dicas de Solução de Problemas
Problema	Solução
No module named tkinter	Reinstale o Python com Tkinter incluso ou use pip install tk
Arquivo não encontrado	Verifique se os três arquivos estão na mesma pasta
Executável não abre	Tente rodar via terminal para ver mensagens de erro
Tabela não atualiza	Certifique-se de que clientes.db está na mesma pasta do .exe

🎓 Para Alunos: O que você aprende com esse projeto?
Python: Classes, funções, organização modular

SQLite: Estrutura de tabelas, comandos SQL, segurança com parâmetros

Tkinter: Criação de GUIs, eventos e controle de widgets

Boas práticas: Separação de responsabilidades, reuso de código

Distribuição: Criar executáveis com PyInstaller

🌟 Próximos Passos
Aqui vão algumas sugestões de melhorias:

🔐 Validação de CPF (formato correto e único)

📤 Exportar clientes para CSV

🔄 Botão de "Recarregar" clientes

🎨 Melhorias visuais com cores e ícones

🛠️ Desenvolvido por BRYAN EDUARDO
"# agenda_clientes" 
"# agenda_clientes" 
"# agenda_clientes" 
"# agenda_clientes" 
