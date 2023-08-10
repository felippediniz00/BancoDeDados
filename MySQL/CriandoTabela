CREATE DATABASE db_empresa;
use db_empresa;


CREATE TABLE Employees (
 --Atributos    
    id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    birth_date DATE,
    hire_date DATE,
    job_title VARCHAR(100),
    department VARCHAR(100),
    salary DECIMAL(10, 2)
);


INSERT INTO Employees (first_name, last_name, birth_date, hire_date, job_title, department, salary)
VALUES
    ('João', 'Silva', '1990-05-15', '2015-03-10', 'Desenvolvedor', 'TI', 5000.00),
    ('Maria', 'Santos', '1985-08-20', '2010-09-22', 'Gerente de Vendas', 'Vendas', 7500.00),
    ('Pedro', 'Ferreira', '1992-11-03', '2018-07-05', 'Analista de Marketing', 'Marketing', 4500.00),
    ('Ana', 'Oliveira', '1988-02-10', '2009-12-15', 'Engenheira de Produção', 'Produção', 6000.00),
    ('Carlos', 'Ribeiro', '1995-07-28', '2021-02-18', 'Estagiário', 'RH', 2500.00),
    ('Fernanda', 'Martins', '1991-08-08', '2014-06-20', 'Engenheira de Software', 'TI', 5500.00),
    ('Rafael', 'Pereira', '1987-08-12', '2011-04-15', 'Gerente de Projetos', 'TI', 7000.00),
    ('Isabela', 'Rodrigues', '1993-05-03', '2019-09-10', 'Analista Financeiro', 'Financeiro', 4800.00),
    ('Gabriel', 'Almeida', '1990-05-18', '2015-01-25', 'Analista de RH', 'RH', 4200.00),
    ('Luana', 'Carvalho', '1994-08-05', '2020-03-12', 'Designer Gráfico', 'Design', 4000.00),
    ('Luis', 'Gomes', '1989-05-09', '2013-11-08', 'Desenvolvedor Web', 'TI', 5200.00);


SELECT * 
FROM Employees
WHERE YEAR(CURDATE()) - YEAR(birth_date) < 30;


SELECT MONTH(birth_date) AS birth_month, COUNT(*) AS num_birthdays
FROM Employees
GROUP BY birth_month
ORDER BY num_birthdays DESC
LIMIT 1;
