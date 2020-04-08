# DatabaseEssential-MySQL

A simple codebase to implement Backend to your Unity App or Games.

# Classes 

**DatabaseManager.cs**  Core class which contains all functions to initialize and command.

**ServerConfiguration.cs**  ScriptableObject Class, that allow to create multiple profile for different servers and change any server config easily.

**DatabaseTest.cs**  A test class to check the codebase. 


# Useful Functions 


```c# 
public bool Close() 
//Example
DatabaseEssential.DatabaseManager.instance.Close();
``` 
To close any existing connection from Server. 

```public string Query(string statement)``` To execute any Reader SQL Statement 

```public void NonQuery(string statement)``` To execute Non-Query SQL Command

```public void InsertRecord(string tableName, string keys, string values)``` To Insert Record(s) to Table 

```public void DeleteRecord(string tableName, string condition)``` To Delete Record(s) from Table

```public void UpdateRecord(string tableName, string condition)``` To Updata Data in Database

```public List<string>[] SelectAllRecord(string tableName, string columnName)``` To Fetch All Records from Table according to column name

```public int Count(string tableName)``` To count records of Table