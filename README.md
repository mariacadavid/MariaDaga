# MariaDaga (GeneBank to SQL)

Mariadaga is a tool to upload GeneBank file information into a SQL database.

The SQLite database contains 4 tables: organism, extended comments, protein, sequence. (For a better understanding of its structure refer to the file "Diagram_database.png")

Here you can find the main script (mariadaga.py) and source scripts (in lib directory: flatlayer.py, sqlitelayer.py and transfer.py) for the program which is writen in python.

To run the tool you must have all the scripts (here provided), the SQL database (here provided as "GeneBank_DataBase.db") and your own directory with the genebank (.gbff) files of interest. 


Command line for console: 

> python3 mariadaga.py "data_base_path" "gbff_files_path" "verbose_mode" "delete_mode"

- verbose_mode must be "Y" when you want the program to show indications of what it is processing, else "N".
- delete_mode must be "Y" when you want to delete pre-existent records in the database before processing new files, to keep previous records in the database and  add new records delete_mode must be "N".



