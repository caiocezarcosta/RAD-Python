apresentamos um programa que faz a inserção de dados na tabela AGENDA :
01 import psycopg2
02 conn = psycopg2.connect(database = "postgres", user = "postgres", password = " senha123", host =
"127.0.0.1", port = "5432")
03 print ("Conexão com o Banco de Dados aberta com sucesso!")
04 cur = conn.cursor()
05 cur.execute("""INSERT INTO public."AGENDA" ("id", "nome", "telefone") VALUES (1, 'Pessoa1',
'02199999999')""")
06 conn.commit()
07 print("Inserção realizada com sucesso!");
08 conn.close()

A respeito do código apresentado, selecione a opção correta.
a) A única forma de executar uma operação de inserção em uma tabela é conforme a linha 5.
b) Se o comando da linha 8 for removido, o programa vai funcionar corretamente.
c) Esse programa está preparado para tratar exceções de conexão com o banco de dados.
d) O cursor que é instanciado na linha 4 é fundamental para que o programa possa funcionar
corretamente.
e) Esse código está implementado usando programação orientada a objetos

Resposta: Letra (D)

Questão 2) O Python possui diversos frameworks para fazer operações em um banco de dados.
Entre esses frameworks está o psycopg2 que faz a interface com o Postgres.
Em relação ao psycopg2, selecione a opção correta:
a) Permite a criação de tabelas e a execução dos comandos de inserção, exclusão, modificação e
consulta no banco de dados.
b) Faz interface com outros Sistemas Gerenciadores de Banco de Dados (SGBDs), como o MySQL e
Oracle.
c) Para ser utilizado, é fundamental programar orientado a objetos.
d) Os programas que utilizam o psycopg2 só vão funcionar se as exceções forem tratadas
explicitamente.
e) Os programas que utilizam o psycopg2 devem estar implementados seguindo a programação
estruturada.

Resposta: Letra (A)