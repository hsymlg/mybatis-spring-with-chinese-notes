MyBatis Spring Adapter
======================

[![Java CI](https://github.com/mybatis/spring/actions/workflows/ci.yaml/badge.svg)](https://github.com/mybatis/spring/actions/workflows/ci.yaml)
[![Coverage Status](https://coveralls.io/repos/mybatis/spring/badge.svg?branch=master&service=github)](https://coveralls.io/github/mybatis/spring?branch=master)
[![Maven central](https://maven-badges.herokuapp.com/maven-central/org.mybatis/mybatis-spring/badge.svg)](https://maven-badges.herokuapp.com/maven-central/org.mybatis/mybatis-spring)
[![Sonatype Nexus (Snapshots)](https://img.shields.io/nexus/s/https/oss.sonatype.org/org.mybatis/mybatis-spring.svg)](https://oss.sonatype.org/content/repositories/snapshots/org/mybatis/mybatis-spring/)
[![License](http://img.shields.io/:license-apache-brightgreen.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

![mybatis-spring](http://mybatis.github.io/images/mybatis-logo.png)

MyBatis-Spring adapter is an easy-to-use Spring bridge for MyBatis sql mapping framework.

Supported Versions
------------------

- master (2.1.x) - Support Spring 6(keep backward compatibility for Spring 5)
- 2.0.x - Support for Java 8, Spring 5, and Junit 5 plus other java 8 requirements
- 1.3.x - Continued support for Java 6 and 7

Essentials
----------

* [See the published docs](http://mybatis.github.io/spring/)
* [See the snapshot docs](src/site/markdown) (Note: may contain explanation of unreleased features)

SqlSessionFactoryBean 遵循 Spring FactoryBean 的定义，使得 SqlSessionFactory 注册在 Spring 容器中。
SqlSessionTemplate 是 SqlSession 另一种线程安全版本的实现，并且能够更好地与 Spring 事务管理集成。
MapperFactoryBean 是生成 mapper 接口代理类的 SqlSessionTemplate 版本实现。
MapperScannerConfigurer 简化了生成 mapper 接口代理的逻辑，指定扫描的包即可将生成 mapper 接口代理类并注册为 Spring bean。