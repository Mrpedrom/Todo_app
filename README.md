Se trata de um projeto de lista de tarefas para entender melhor sobre Java Web em geral ou Java EE, integrando tecnologias como JDBC, MySQL, Java, JSP, JSF, Servlets e outros conceitos.

📌 Requisitos
Antes de utilizar este projeto, é necessário ter instalado:

Uma IDE como Eclipse, NetBeans ou Visual Studio.
Apache Tomcat 9.0.95.
Java SE 21 ou uma versão Java 8+.
jstl-1.2.jar.

📌 Funcionalidades
Por ser uma lista de tarefas (To-Do), ele desempenha funções básicas como:

Cadastro → Você precisa se cadastrar com um e-mail e uma senha.
Acesso ao Menu → Onde é possível visualizar a lista de tarefas.
Adicionar tarefa → Criar e adicionar uma nova tarefa.
Editar tarefa → Modificar uma tarefa existente.
Remover tarefa → Excluir uma tarefa.
Logout → Sair da aplicação.
Validação de Campos → Se algum campo obrigatório não for preenchido, será exibida uma mensagem de aviso.
Visualização da Lista de Tarefas → Exibe todas as tarefas cadastradas.

📌 Melhorias Futuras
Substituir JSP por AJAX.
Melhorar a configuração do Maven e do Hibernate.
Criar um Front-End mais adequado.
Melhorar a lógica do código e o direcionamento dos links.
Comentar melhor o código para facilitar a manutenção.

📂 Diretórios e Explicações

Pacote principal da aplicação (src/main/java/todoapp)
📂 dao/ (Data Access Object - DAO) → Responsável pelo acesso ao banco de dados.
LoginDao.java → Gerencia a autenticação dos usuários.
TodoDao.java → Gerencia operações relacionadas às tarefas.
TodoDaoImpl.java → Implementação da interface TodoDao.
UserDao.java → Gerencia operações dos usuários no banco de dados.
📂 model/ → Contém as classes modelo que representam os dados da aplicação.
LoginBean.java → Representa os dados de login do usuário.
Todo.java → Representa uma tarefa na lista de afazeres.
User.java → Representa um usuário no sistema.
📂 utils/ → Contém utilitários para suporte à aplicação.
JDBCUtils.java → Gerencia a conexão com o banco de dados.
📂 web/ → Contém os controladores (Servlets) que gerenciam as requisições HTTP.
LoginController.java → Processa as requisições de login.
TodoController.java → Processa as requisições relacionadas às tarefas.
UserController.java → Gerencia as requisições relacionadas aos usuários.
📂 Interface da Aplicação (src/main/webapp/)
📂 login/
index.jsp → Página inicial.
login.jsp → Página de login do usuário.
📂 register/
register.jsp → Página de registro de novos usuários.
📂 todo/
todo-form.jsp → Formulário para criar/editar tarefas.
todo-list.jsp → Lista de tarefas cadastradas.
📂 WEB-INF/
lib/ → Contém as bibliotecas utilizadas, como jstl-1.2.jar (JSTL para JSP).

web.xml → Arquivo de configuração da aplicação web.

Error.jsp → Página para exibir erros do sistema.

📄 Banco de Dados
script.sql → Contém os scripts SQL para criar e popular o banco de dados.
