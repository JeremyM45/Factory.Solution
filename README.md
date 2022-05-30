
# _Factory_

#### By _**Jeremy Martin**_

#### _A Webpage that displays and edits databases of engineers licensed to work on machines and the machines with the engineers who are licensed to work on them_

## Technologies Used

* C#
* MySQL
* MySQL Workbench
* Entity
* .NET 5.0

## Description

This web page will initially display a splash page were you can click on either a machine or engineer to see their details including the machines they are licensed to repair (engineers) or the engineers licensed to repair them (machines). There are also links to the list of engineers or machines with the ability to add machines/engineers from their respective list pages. On the list pages you can also click on an engineer or machine to go to their details page (just like from the splash page). In the details page there are links you can click to edit or delete the specific engineer or machine as wells as buttons to remove a machine's pair with an engineer or vice versa. 

## Setup/Installation Requirements

### Getting Started

* Clone repo from GitHub using this link (https://github.com/JeremyM45/Factory.Solution)

* Navigate to the Factory.Solution folder in terminal
```
(Users/Username/Desktop/Factory.Solution)
```
* cd into the Factory folder
```
cd Factory
```
* Add an appsettings.json file in the Factory folder

* In the appsettings.json file add these lines of code with your MySQL password were [Your Password Here] is.

```
{
"ConnectionStrings": {
"DefaultConnection": "Server=localhost;Port=3306;database=jeremy_martin;uid=root;pwd=[Your Password Here];"
}
}
```

### Setting up database

* Open MySQL Workbench and sign in

* Under the management tab in the Navigator click on Data Import/Restore

* Click the Import From Self Contained File radio button and input the path to jeremy_martin.sql file in Factory.Solution folder

```
../Factory.Solution/jeremy_martin.sql
```

* In the Default Schema to be Imported To section click the new button and name the schema jeremy_martin (you can name it something else if you change the database path in the appsettings.json file)

* Then click the Start Import button

* Once the schema has been imported refresh your Schemas list in the Navigator to see the new schema

### Restore and Run

* Type dotnet retore in terminal while in the Factory folder
```
dotnet restore
```
* Then type dotnet run in the terminal while still in the Factory folder
```
dotnet run
```

## Known Bugs

*  _No known bugs_

## License

[MIT](https://opensource.org/licenses/MIT)

Copyright (c) _2022_  _Jeremy Martin_