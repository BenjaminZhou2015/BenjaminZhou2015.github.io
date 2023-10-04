Use Testmsdb
CREATE TABLE Persons (
    Id INT PRIMARY KEY,
    Name NVARCHAR(50),
    Age int
);

INSERT INTO Persons (Id, Name, Age)
VALUES
    (1, 'Abe', 10),
    (2, 'Ben', 20),
    (3, 'Emily', 30),
    (4, 'Mike', 40);

	INSERT INTO Persons (Id, Name, Age)
VALUES
    (5, 'Abe', 10)
 
 select * from Persons

 select distinct Name,  Age from Persons

