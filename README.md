create database db_clinica_bsb;
use db_clinica_bsb;
create table tb_paciente(
id int not null auto_incremente,
nome varchar(30),
primary key(id));
alter table tb_paciente add sexo enum('f','m');
alter table tb_paciente add endereco varchar(30);
alter table tb_paciente drop primary key;
alter table tb_paciente add id int not null auto_incremente;
alter table tb_paciente add primary key (id);
alter table tb_paciente change endereco endereco varchar(150);
insert into tb_paciente values(null , 'josyane','f','asa norte');
insert into tb_paciente values(null , 'ingrid','f','taguatinga sul');
insert into tb_paciente values(null , 'joao vitor','m','taguatinga sul');
insert into tb_paciente values(null , 'tiago','m','aguas claras');
insert into tb_paciente values(null , 'marta','f','ceilandia');
