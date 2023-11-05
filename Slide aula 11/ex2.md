Questão 2) O Python possui diversos frameworks para trabalhar com banco de dados. Um desses
frameworks é o psycopg2 que faz interface com o Postgres. Observe o programa abaixo.
import psycopg2
conn=psycopg2.connect(database="postgres", user="postgres", password="senha123", host="127.0.0.1",
port="5432")
print ("Conexão com o Banco de Dados aberta com sucesso!")
cur = conn.cursor()
cur.execute("""select * from public."AGENDA" where "id" = 1""")
registro = cur.fetchone()
print(registro)
conn.commit()
print("Seleção com sucesso!");
conn.close()
Agora, selecione a opção correta
a respeito do programa :
a) O programa garante que sempre vai retornar dados.
b) O programa realiza uma consulta na tabela AGENDA onde o atributo id
da tabela seja igual a 1.
c) O código está preparado para tratar possíveis exceções de execução.
d) O código está implementado u

Resposta: Alternativa B