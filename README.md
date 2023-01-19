# Banco-de-Dados
## Modelo Conceitual e Lógico de Banco de Dados
#### Trabalho individual do Módulo 4 PROGRAMADORES CARIOCAS

Uma empresa está pensando em lançar um novo sistema de acompanhamento e para isso precisa de uma modelagem de banco de dados que armazena **_cursos, alunos e turmas_**.

**⇨ Existem outras entidades além dessas três?**
Sim: Professor e Disciplina

**⇨ Quais são os principais campos e tipos?**
Entidades e atributos, contendo chaves primárias (PK) e estrangeiras (FK). Uma entidade é um conjunto de informações sobre um determinado conceito e toda entidade possuem atributos que possuem informações que a referenciam.

As tabelas possuem **campos** como código da tabela, nome, especialidade e os **tipos** variam entre _varchar_ (somente textos), _int_ (números inteiros) e _date_ (data).

**⇨ Como essas entidades estão relacionadas?** Através das cardinalidades. Nela são definidos os graus de relação entre duas entidades ou tabelas. Existem 3 níveis de relacionamento:

(1,1) *um-para-um*

(1,n) *um-para-muitos*

(n,n) *muitos-para-muitos*

## MODELO CONCEITUAL
O modelo conceitual foi criado na plataforma [Diagram Software and Flowchart Maker](https://www.diagrams.net)

![image](https://user-images.githubusercontent.com/112867913/213447237-a0b66753-6a7d-44c2-b032-8205deef1255.png)

## MODELO LÓGICO
O modelo lógico foi desenvolvido no programa PHP MyAdmin (Xampp)

![image](https://user-images.githubusercontent.com/112867913/213450541-81f5bc7f-8507-414e-8646-04fadb6eed78.png)


#### Estruturação antes da diagramação


- Curso (cod_curso(PK), nome, tipo)

- -- Aluno (cod_aluno (PK), cod_curso(FK), matrícula, nome, endereço, telefone)

- -- Turma (cod_turma(PK), cod_disc(FK), cod_curso(FK), data_inicio)

- -- Disciplina (cod_disc(PK), ementa, cont_prog, cod_prof(FK))

- Professor (cod_prof(PK), nome, sexo, especialidade)
