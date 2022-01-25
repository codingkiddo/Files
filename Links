https://github.com/vinoddsce/JavaExample11.git


export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-17.0.1.jdk/Contents/Home
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_311.jdk/Contents/Home





java.sql.SQLNonTransientConnectionException: Public Key Retrieval is not allowed
	at com.mysql.cj.jdbc.exceptions.SQLError.createSQLException(SQLError.java:110)
	at com.mysql.cj.jdbc.exceptions.SQLError.createSQLException(SQLError.java:97)
	at com.mysql.cj.jdbc.exceptions.SQLExceptionsMapping.translateException(SQLExceptionsMapping.java:122)
	at com.mysql.cj.jdbc.ConnectionImpl.createNewIO(ConnectionImpl.java:835)
	at com.mysql.cj.jdbc.ConnectionImpl.<init>(ConnectionImpl.java:455)
	at com.mysql.cj.jdbc.ConnectionImpl.getInstance(ConnectionImpl.java:240)
	at com.mysql.cj.jdbc.NonRegisteringDriver.connect(NonRegisteringDriver.java:207)
	at java.sql/java.sql.DriverManager.getConnection(DriverManager.java:681)
	at java.sql/java.sql.DriverManager.getConnection(DriverManager.java:229)
	at com.jdbc.learning.MainApp.main(MainApp.java:37)



package com.spring.config;

import javax.sql.DataSource;

import org.apache.commons.dbcp2.BasicDataSource;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.context.annotation.PropertySource;
import org.springframework.core.env.Environment;

import com.spring.beans.employee.EmployeeManager;

@Configuration
//@PropertySource("classpath:database.properties")
public class JavaConfig {

//	@Autowired
//    private Environment env;
	
	@Bean
	public EmployeeManager getEmployeeManager() {
		return new EmployeeManager();
	}
	
//	@Bean
//	public DataSource getDataSource() {
//		BasicDataSource ds = new BasicDataSource();
//		ds.setDriverClassName(env.getProperty("MYSQL_DB_DRIVER_CLASS"));
//		ds.setUrl(env.getProperty("MYSQL_DB_URL"));
//		ds.setUsername(env.getProperty("MYSQL_DB_USERNAME"));
//		ds.setPassword(env.getProperty("MYSQL_DB_PASSWORD"));
//		ds.setInitialSize(10); // The initial number of connections that
//        // are created when the pool is started.
//		ds.setMaxTotal(20); // The maximum number of active connections
//        // that can be allocated from this pool
//		return ds;
//	}
	
}
