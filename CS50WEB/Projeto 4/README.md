# Network

## Descrição
Network é um site de rede social semelhante ao Threads, permitindo que usuários publiquem posts, sigam outros usuários e curtam postagens. O projeto foi desenvolvido utilizando **Django**, **Python**, **JavaScript**, **HTML** e **CSS**.

## Funcionalidades
- **Novo Post**: Usuários autenticados podem escrever e postar conteúdo.
- **Todos os Posts**: Exibição de todas as postagens em ordem cronológica reversa.
- **Perfil do Usuário**:
  - Exibição do número de seguidores e seguidos.
  - Lista de postagens do usuário em ordem cronológica reversa.
  - Opção para seguir ou deixar de seguir outros usuários.
- **Seguindo**: Exibição das postagens apenas dos usuários seguidos.
- **Paginação**: Exibição de posts em lotes de 10 por página.
- **Edição de Posts**:
  - Usuários podem editar suas próprias postagens.
  - Atualização assíncrona sem recarregar a página.
- **Curtir e Descurtir Posts**:
  - Usuários podem curtir e descurtir postagens de outros.
  - Atualização dinâmica do número de curtidas.

## Instalação e Configuração
1. Clone o repositório:
   ```sh
   git clone https://github.com/renansousasilva1/network.git
   cd network
   ```
2. Instale as dependências:
   ```sh
   pip install -r requirements.txt
   ```
3. Realize as migrações do banco de dados:
   ```sh
   python manage.py makemigrations network
   python manage.py migrate
   ```
4. Inicie o servidor Django:
   ```sh
   python manage.py runserver
   ```
5. Acesse o site em [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## Estrutura do Projeto
```
network/
│── migrations/           # Arquivos de migração do banco de dados
│── static/               # Arquivos estáticos (CSS, JS, imagens)
│── templates/            # Templates HTML
│── __init__.py
│── admin.py              # Configuração do painel administrativo
│── apps.py               # Configuração do app Django
│── models.py             # Modelos do banco de dados
│── tests.py              # Testes automatizados
│── urls.py               # Rotas do aplicativo
│── views.py              # Lógica das views
```

## Modelos
### **Usuário**
O projeto utiliza o modelo `User` do Django (`AbstractUser`) e permite extensões para armazenar mais informações, como seguidores e seguidos.

### **Post**
Cada post possui um autor, conteúdo, data de criação e número de curtidas.

### **Relacionamento de Seguidores**
Tabela que armazena os relacionamentos de seguidores entre usuários.

## Tecnologias Utilizadas
- **Backend**: Django, Python
- **Frontend**: HTML, CSS, JavaScript
- **Banco de Dados**: SQLite (padrão, mas pode ser alterado para PostgreSQL ou MySQL)
- **Autenticação**: Django Authentication System
- **Paginação**: Django Paginator
- **Estilização**: Bootstrap

## Melhorias Futuras
- Implementar upload de imagens nos posts.
- Melhorar o design responsivo.
- Adicionar comentários nos posts.

## Licença
Este projeto é licenciado sob a licença MIT.

## Autor
Desenvolvido como parte do curso **CS50W**.

