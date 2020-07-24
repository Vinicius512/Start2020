# Start2020
Projeto de banco de  da



create database taxi99;

integer
create table motorista(
Matricula int UNIQUE, cpf varchar(11) PRIMARY KEY, Nome varchar(255), 
Veiculo_Placa varchar(7), endereco varchar(255)
);

INSERT into motorista 
( Matricula, cpf, Nome, Veiculo_Placa, enderenco)
VALUES(1, 22577798710, 'José', 'POI0989', 'Rua A');

INSERT into motorista
( Matricula, cpf, Nome, Veiculo_Placa, enderenco)
VALUES(2, 22577798711, 'Davi', 'PLK1237', 'Rua B');

INSERT into motorista
( Matricula, cpf, Nome, Veiculo_Placa, enderenco)
VALUES(3, 22577798712, 'Felipe', 'PAF7652', 'Rua C');

INSERT into motorista
( Matricula, cpf, Nome, Veiculo_Placa, enderenco)
VALUES(4, 22577798713, 'Luiza', 'PSG4731', 'Rua D');

INSERT into motorista 
( Matricula, cpf, Nome, Veiculo_Placa, enderenco)
VALUES(5, 22577798714, 'Wagner', 'PLR2398', 'Rua E');






create table viagens(
Matricula_motorista int, cpf_cliente varchar(11),
endereco_inicial varchar(255), endereco_final varchar(255), valor decimal(9,2), data_viagem date
);

INSERT into viagens 
( Matricula_motorista, cpf_cliente, endereco_inicial, endereco_final, valor, data_viagem)
VALUES(1, 12345678901, 'Rua A', 'Rua T', '98.00', '2020-01-01');

INSERT into viagens 
( Matricula_motorista, cpf_cliente, endereco_inicial, endereco_final, valor, data_viagem)
VALUES(2, 123456789012, 'Rua B', 'Rua V', '150.00', '2020-02-02');

INSERT into viagens 
( Matricula_motorista, cpf_cliente, endereco_inicial, endereco_final, valor, data_viagem)
VALUES(3, 12345678903, 'Rua C', 'Rua P', '78.00', '2020-03-03');

INSERT into viagens 
( Matricula_motorista, cpf_cliente, endereco_inicial, endereco_final, valor, data_viagem)
VALUES(4, 12345678904, 'Rua D', 'Rua H', '25.00', '2020-04-04');

INSERT into viagens 
( Matricula_motorista, cpf_cliente, endereco_inicial, endereco_final, valor, data_viagem)
VALUES(5, 12345678905, 'Rua E', 'Rua K', '40.00', '2020-05-05');








create table clientes(
Nome varchar(255), cpf varchar(11) PRIMARY KEY, endereço varchar(255)
);


INSERT into clientes 
( Nome, cpf, endereço)
VALUES('Luis', 12345678901, 'Rua A');

INSERT into clientes 
( Nome, cpf, endereço)
VALUES('Carlos', 12345678902, 'Rua B');

INSERT into clientes 
( Nome, cpf, endereço)
VALUES('Karol', 12345678903, 'Rua C');

INSERT into clientes 
( Nome, cpf, endereço)
VALUES('Victor', 12345678904, 'Rua D');

INSERT into clientes 
( Nome, cpf, endereço)
VALUES('Maria', 12345678905, 'Rua E');




SELECT cpf_cliente FROM viagens WHERE valor > 50.00
SELECT * FROM viagens WHERE data_viagem BETWEEN '2020-01-01' AND '2020-04-04'
SELECT cpf_cliente FROM viagens WHERE valor > 100.00 OR (valor < 80.00 AND valor > 40.00)
