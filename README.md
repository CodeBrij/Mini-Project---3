package login;
import java.sql.Connection;
import java.sql.DriverManager;

public class db {
    
    public static Connection mycon(){
    Connection con = null ;
    try{
     Class.forName("com.mysql.jdbc.Driver");
    con =DriverManager.getConnection("jdbc:mysql://127.0.0.1:3306/login","root","");
    }catch(Exception e){
System.out.println(e);
    }
        return con;
    }
}
