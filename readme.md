Roluri
=======

Rolurile dispobibile sunt:
	STUDENT, 					//student
	LEADER, 					//sef de grupa
	TEACHER, 					//profesor, seminarist, asistent
	SECRETARY, 					//secretariat
	BOARD, 						//conducerea facultatii
	ADMINISTRATOR 				//administrator platforma


API public:

 /listgroups

Returneaza lista grupelor
Exemplu raspuns: [{"id":1,"name":"343"},{"id":2,"name":"344"}]


/listusers

Returneaza lista userilor existenti
Exemplu raspuns:
[
	{"firstName":"Timofte","lastName":"Ciprian","groupId":"1","id":"1","username":"ciprian"},
	{"firstName":"Susnea","lastName":"Radu","groupId":"2","id":"2","username":"radu"},
	{"firstName":"Nita","lastName":"Alexandra","groupId":"1","id":"3","username":"alexandra"},
	{"firstName":"Tofan","lastName":"Ionut","groupId":"1","id":"4","username":"ionut"},
	{"firstName":"Popa","lastName":"Vlad","groupId":"1","id":"5","username":"vlad"}
]





===================================

Model
-----

Tabel fminews_user //tabelul userilor

fminews=> select * from fminews_user;
 id | firstname | lastname  | password | username  | groupid
----+-----------+-----------+----------+-----------+---------
  1 | Timofte   | Ciprian   | 1234     | ciprian   |       1
  2 | Susnea    | Radu      | 1234     | radu      |       2
  3 | Nita      | Alexandra | 1234     | alexandra |       1
  4 | Tofan     | Ionut     | 1234     | ionut     |       1
  5 | Popa      | Vlad      | 1234     | vlad      |       1
(5 rows)


Tabel fminews_group  // tabelul grupelor

fminews=> select * from fminews_group;
 id | name
----+------
  1 | 343
  2 | 344
(2 rows)