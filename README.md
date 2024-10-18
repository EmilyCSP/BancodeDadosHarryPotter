# BancodeDadosHarryPotter
Estes são alguns comandos práticados e treinados após um curso recente de Mysql utilizando workbench. 


CREATE DATABASE hogwarts;
USE hogwarts;

CREATE TABLE alunos (
    id_aluno INT PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(50) NOT NULL,
    casa VARCHAR(20) NOT NULL,
    ano INT
);
CREATE TABLE professores (
    id_professor INT PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(50) NOT NULL,
    disciplina VARCHAR(50) NOT NULL,
    casa VARCHAR(20)
);

CREATE TABLE disciplinas (
    id_disciplina INT PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(50) NOT NULL
);

INSERT INTO alunos (nome, casa, ano)
VALUES
    ('Harry Potter', 'Grifinória', 1),
    ('Hermione Granger', 'Grifinória', 1),
    ('Ronald Weasley', 'Grifinória', 1);
    
    INSERT INTO professores (nome, disciplina, casa)
VALUES
    ('Severo Snape', 'Poções', 'Sonserina'),
    ('Minerva McGonagall', 'Transfiguração', 'Grifinória');
    
    INSERT INTO disciplinas (nome)
VALUES
    ('Poções'),
    ('Transfiguração'),
    ('Defesa contra as Artes das Trevas');
    
    SELECT * FROM alunos WHERE casa = 'Grifinória';
    
    SELECT * FROM professores WHERE disciplina = 'Poções';
       
INSERT INTO alunos (nome, casa, ano)
VALUES
    ('Harry Potter', 'Grifinória', 1);
    
    DELETE FROM alunos WHERE id_aluno = 5;
