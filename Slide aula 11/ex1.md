1) PostgreSQL é um dos banco de dados mais utilizados no mundo, por ser opensource
torna-se uma ótima opção aos banco de dados pagos como Oracle e SqlServer. O PSYCOPG é
considerado o adaptador mais utilizado para conexões com o PostgreSQL. A forma correta de abrir
conexão com o PSYCOPG é:
a) import psycopg con = psycopg.open(host='localhost', database='exemplo', user='postgres',
password='postgres123')
b) import psycopg2 con = psycopg2.open(host='localhost', database='exemplo', user='postgres',
password='postgres123')
c) import psycopg con = psycopg.connect(host='localhost', database='exemplo', user='postgres',
password='postgres123')
d) import psycopg2 con = psycopg2.postgres(host='localhost', database='exemplo', user='postgres',
password='postgres123')
e) import psycopg2 con = psycopg2.connect(host='localhost', database='exemplo', user='postgres',
password='postgres123')

Resposta: Alternativa C