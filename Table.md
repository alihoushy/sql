Sample `Users` Table
```
| UserId | UserName      | MobileNumber | Email              | NationalCode   | Country       | City        | IsSubscribed |
|--------|---------------|--------------|--------------------|----------------|---------------|-------------|--------------|
| 1      | Ali Nikravan  | +989131313   | nikravan@gmail.com | 2525252525     | Iran          | Tehran      | 1            |
| 2      | Farid Talebi  | +989121212   | talebi@gmail.com   | 4545454545     | Armenia       | Yerevan     | 1            |
| 3      | Iman Hosseini | +989141414   | hosseini@gmail.com | 6565656565     | United States | Los Angeles | 0            |
| 4      | Elaheh Yazdi  | +989151515   | yazdi@gmail.com    | 7575757575     | France        | Paris       | 1            |
| 5      | Sorena Yasini | +989161616   | yasini@gmail.com   | 9595959595     | Sweeden       | Stockholm   | 0            |
```

`CREATE TABLE` command
```
CREATE TABLE Users (
    UserId INT PRIMARY KEY,
    UserName VARCHAR(255),
    MobileNumber VARCHAR(15),
    Email VARCHAR(255),
    NationalCode VARCHAR(10),
    Country VARCHAR(255),
    City VARCHAR(255),
    IsSubscribed INT
);
```

`INSERT DATA` command
```
INSERT INTO Users (UserId, UserName, MobileNumber, Email, NationalCode, Country, City, IsSubscribed)
VALUES
(1, 'Ali Nikravan', '+989131313', 'nikravan@gmail.com', '2525252525', 'Iran', 'Tehran', 1),
(2, 'Farid Talebi', '+989121212', 'talebi@gmail.com', '4545454545', 'Armenia', 'Yerevan', 1),
(3, 'Iman Hosseini', '+989141414', 'hosseini@gmail.com', '6565656565', 'United States', 'Los Angeles', 0),
(4, 'Elaheh Yazdi', '+989151515', 'yazdi@gmail.com', '7575757575', 'France', 'Paris', 1),
(5, 'Sorena Yasini', '+989161616', 'yasini@gmail.com', '9595959595', 'Sweeden', 'Stockholm', 0);
```
