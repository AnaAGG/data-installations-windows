# 5. SQL

**5.1. Installation**

To install mySQL in our computer we will need to install two differents programs: 

- **5.5.1 SQL Server**  

    - In the terminal: 

            sudo apt update sudo apt install mysql-server
            sudo /etc/init.d/mysql start # to elevate the server
    
        ⚠️ When you run this last code you will get a warning in the terminal. Nothing happens, we can continue working ⚠️ 
    - Configurar SQL

            # In the terminal
            sudo mysql -u root -p

        ```SQL
        USE mysql; 

        ALTER USER 'root'@'localhost' 
        IDENTIFIED WITH mysql_native_password BY 'admin';
        #Substitute 'admin' by your password if you want
        FLUSH PRIVILEGES; 
        
        QUIT;
        ```

- **5.5.2 Workbench**   
    To install Workbench we should open our browser and go to the mySQL [website](https://www.anaconda.com/products/individual)