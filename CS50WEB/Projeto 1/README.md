# Wiki - CS50 Web Programming with Python and JavaScript

## Descrição
Este projeto faz parte do curso [CS50's Web Programming with Python and JavaScript](https://cs50.harvard.edu/web/) e tem como objetivo criar uma enciclopédia online semelhante à Wikipedia. As entradas da enciclopédia são armazenadas em arquivos Markdown e são convertidas para HTML dinâmicamente ao serem acessadas.

## Funcionalidades
- **Página Inicial**: Lista todas as entradas da enciclopédia, permitindo acesso direto ao conteúdo.
- **Busca**: Permite ao usuário buscar uma entrada exata ou visualizar resultados que contenham a consulta.
- **Criação de Novas Páginas**: Usuários podem adicionar novas entradas para a enciclopédia em Markdown.
- **Edição de Entradas**: Possibilidade de editar uma entrada existente diretamente na interface web.
- **Página Aleatória**: Opção para carregar aleatoriamente uma entrada da enciclopédia.
- **Conversão de Markdown para HTML**: O conteúdo em Markdown é convertido para HTML para exibição na página.

## Tecnologias Utilizadas
- **Python** (Django Framework)
- **HTML & CSS** (Bootstrap para estilização)
- **JavaScript**
- **Markdown2** (Para conversão de Markdown para HTML)

## Como Executar o Projeto
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/wiki-cs50w.git
   cd wiki-cs50w
   ```

2. Crie e ative um ambiente virtual:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

4. Execute a aplicação Django:
   ```bash
   python manage.py runserver
   ```

5. Acesse a aplicação no navegador: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Estrutura do Projeto
```
wiki/
│── encyclopedia/          # Aplicativo principal
│   ├── templates/        # Templates HTML
│   ├── static/           # Arquivos estáticos (CSS, JS)
│   ├── views.py          # Lógica das views
│   ├── urls.py           # Configuração de rotas
│   ├── util.py           # Funções auxiliares para manipulação de entradas
│── entries/              # Diretório contendo as entradas em Markdown
│── manage.py             # Comando para executar a aplicação
│── db.sqlite3            # Banco de dados SQLite (se utilizado)
│── requirements.txt      # Lista de dependências do projeto
```

## Melhorias Futuras
- Implementar suporte a imagens nas entradas da enciclopédia.
- Melhorar a interface de edição com um editor Markdown visual.
- Criar um sistema de autenticação para permitir apenas edição por usuários logados.

## Autoria
Este projeto foi desenvolvido como parte do curso **CS50 Web Programming with Python and JavaScript** da HarvardX.



