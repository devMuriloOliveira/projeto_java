<h1>Projeto: Simulação de Pessoas (Aluno e Professor)</h1> <h2>Descrição</h2>
Este projeto é uma simulação simples de um sistema de cadastro de pessoas utilizando a linguagem Java.
O sistema define três classes principais:

<b>Pessoa</b>: Classe base que representa informações comuns a qualquer pessoa.

<b>Aluno</b>: Classe que herda de Pessoa e adiciona informações específicas de um aluno.

<b>Professor</b>: Classe que herda de Pessoa e adiciona informações específicas de um professor.

O projeto também inclui a classe <code>App</code>, responsável por criar objetos e exibir algumas informações no console.

<h2>Estrutura das Classes</h2> <h3>Pessoa</h3>
Classe base que contém atributos comuns a qualquer pessoa:

<b>nome</b> (String) — Nome da pessoa.

<b>sexo</b> (String) — Sexo da pessoa (não pode ser alterado depois de criado).

<b>dataNascimento</b> (String) — Data de nascimento (imutável).

<b>cidadeNatal</b> (String) — Cidade onde nasceu (imutável).

<b>cidadeReside</b> (String) — Cidade onde mora atualmente (pode ser alterada).

<b>Principais métodos:</b>

Getters e setters para acessar ou alterar os atributos.

<code>sexo</code>, <code>dataNascimento</code> e <code>cidadeNatal</code> são atributos finais (não podem ser alterados após a criação).

<h3>Aluno (extends Pessoa)</h3>
Classe que herda de Pessoa e adiciona informações específicas de um aluno:

<b>numeroMatricula</b> (int) — Número de matrícula (imutável).

<b>universidade</b> (String) — Nome da universidade.

<b>curso</b> (String) — Nome do curso.

<b>Principais métodos:</b>

Getters e setters para acessar ou alterar os atributos <code>universidade</code> e <code>curso</code>.

<code>numeroMatricula</code> é final e não pode ser alterado depois de atribuído.

<h3>Professor (extends Pessoa)</h3>
Classe que herda de Pessoa e adiciona informações específicas de um professor:

<b>universidade</b> (String) — Universidade onde trabalha.

<b>departamento</b> (String) — Departamento que pertence.

<b>numeroDaSala</b> (int) — Número da sala onde trabalha.

<b>cpf</b> (String) — CPF do professor (imutável).

<b>Principais métodos:</b>

Getters e setters para <code>universidade</code>, <code>departamento</code> e <code>numeroDaSala</code>.

<code>cpf</code> é final e imutável após a criação do objeto.

<h2>Execução (App)</h2>
No método <code>main</code> da classe <code>App</code>:

Dois objetos <code>Aluno</code> são criados com dados completos.

Dois objetos <code>Professor</code> são criados com dados completos.

Algumas informações dos objetos são exibidas no console usando <code>System.out.println()</code>.

<b>Saída esperada:</b>

yaml
Copiar
Editar
Aluno 1: Murilo, Curso: Engenharia
Aluno 2: Ana, Curso: Medicina
Professor 1: Carlos, Departamento: Computação
Professor 2: Fernanda, Departamento: Biologia
<h2>Observações</h2>
No ambiente do JDoodle (ou similar), não foi possível criar pacotes separados, então todas as classes estão no mesmo arquivo.

Alguns atributos foram definidos como <code>final</code> para garantir a integridade dos dados que não devem ser modificados depois da criação.

O projeto é apenas uma simulação, ideal para fins didáticos sobre herança, atributos finais e organização de classes em Java.

<h2>Tecnologias</h2>
Java 11+

JDoodle (ambiente de testes online)

<h2>Autor</h2>
Desenvolvido por <b>Murilo Oliveira</b>.

