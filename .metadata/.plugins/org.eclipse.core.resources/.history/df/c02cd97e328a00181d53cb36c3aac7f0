package com.dbany.dbany;

import javax.activation.DataSource;

import org.apache.ibatis.session.SqlSessionFactory;
import org.junit.Test;
import org.mybatis.spring.SqlSessionFactoryBean;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.context.annotation.Bean;

@SpringBootApplication
public class DbanyApplication {
	
	@Autowired
	private SqlSessionFactory sqlSession;
	
	@Test
	public void contestLoads(){
		
	
	}
	
	@Test
	public void testSqlSession() throws Exception{
		System.out.println(sqlSession);
	}

	public static void main(String[] args) {
		SpringApplication.run(DbanyApplication.class, args);
	}
	
	@Bean
	public SqlSessionFactory sqlSessionFactory(DataSource dataSource) throws Exception{
		SqlSessionFactoryBean sessionFactory= new SqlSessionFactoryBean();
		sessionFactory.setDataSource((javax.sql.DataSource) dataSource);
		return sessionFactory.getObject();
		
	}
}
 