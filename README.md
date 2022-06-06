<h1 align="center">
  Zinger Framework
</h1>
<h4 align="center">
  Build your own Ecommerce Marketplace 🛍️
</h4>

<p align="center">
  <strong>
    <a href="https://zinger.pw">Website</a>
    |
    <a href="https://zinger-workspace.slack.com/join/shared_invite/zt-e6xt0gc2-nBEy85RhEy7NZv3gWCt6Dg/">Slack</a>
    |
    <a href="https://discord.gg/TqADaXV">Discord</a>
    |
    <a href="https://stackoverflow.com/questions/tagged/zinger">StackOverflow</a>
  </strong>
</p>

<p align="center">
  <a href="LICENSE"><img alt="License" src="https://img.shields.io/github/license/zinger-framework/zinger-spring-server"></a>
  <a href="https://zinger.pw/docs/api"><img alt="Documentation" src="https://img.shields.io/badge/code-documented-brightgreen.svg?style=flat-square"></a>
  <a href="https://github.com/zinger-framework/zinger-spring-server/pulls"><img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square"></a>
</p>

An Open Source Framework for building Hyperlocal Delivery Mobile and Web applications.
Zinger provides developers easy to handle backend for ordering & delivering foods, groceries, fruits, vegetables, medicines, etc.

## Architecture
<img src="https://raw.githubusercontent.com/ddlogesh/zinger-framework-docs/master/website/static/img/zinger/zinger-arch.png" height=75% width=75%/>

#### Zinger Core
&emsp;&emsp;A backend server that exposes the REST API, written in spring boot using MySQL database.

#### Zinger Client
&emsp;&emsp;A customer side application to place and track your orders from multiple store partners near your location. It allows you to browse catalogs of all stores and provides you a seamless shopping experience from order acceptance to last mile delivery.

#### Zinger Partner
&emsp;&emsp;A one-stop solution for store owners to manage and track orders from their clients and it provides an effective order and inventory management solutions.

#### Zinger Admin
&emsp;&emsp;A web console to monitor the zinger client and partner applications. It is a powerful tool to track application performance, manage outlet information and promotes new arrivals to increase brand engagement.

## Database Schema 
Check out the [database schema](https://drawsql.app/zinger-technologies/diagrams/zinger-framework)

## Installation Setup

#### Prerequisites
* Java **8** or newer
* MySQL **8.0.19**
* Spring Boot **2.2.4**

#### Fork Project

* [Fork](https://github.com/zinger-framework/zinger-spring-server/fork) the Main Repository
* Clone the forked repository locally `git clone forked_repo_url`

#### Setup DB

* Open MySQL Workbench
* Run the [DB_INIT.sql](https://github.com/zinger-framework/zinger-spring-server/blob/master/sql/DB_INIT.sql) script to create the tables, indexes and triggers.
* Run the [DB_PROC.sql](https://github.com/zinger-framework/zinger-spring-server/blob/master/sql/DB_PROC.sql) script to create the procedures.
* Run the [DB_INSERT.sql](https://github.com/zinger-framework/zinger-spring-server/blob/master/sql/DB_INSERT.sql) script to populate the database.
* Set your MySQL username and password in [application.properties](https://github.com/zinger-framework/zinger-spring-server/blob/master/src/main/resources/application.properties)

#### Setup Firebase Admin SDK
* Create a new [Firebase](https://console.firebase.google.com/) project 
* Navigate to `Project setting -> Service accounts -> Generate service account -> Generate new private key`
* Set your credentials file path in [application.properties](https://github.com/zinger-framework/zinger-spring-server/blob/master/src/main/resources/application.properties)

## Build & Deploy

#### Eclipse IDE

* Choose `File -> Import -> Maven -> Existing Maven projects`
* Right-click [MainApplication.java](https://github.com/zinger-framework/zinger-spring-server/blob/master/src/main/java/com/food/ordering/zinger/MainApplication.java) and choose `Run As -> Java Application`  

#### IntelliJ IDEA

* Choose `File -> Open` and choose the project location
* Right-click [MainApplication.java](https://github.com/zinger-framework/zinger-spring-server/blob/master/src/main/java/com/food/ordering/zinger/MainApplication.java) and choose `Run MainApplication.main()` 

#### Test

* Visit [localhost:8080](http://localhost:8080) in the browser to check if the setup is successful.
* Test the endpoints in Postman by importing the [API collection](https://github.com/zinger-framework/zinger-spring-server/blob/master/Zinger%20framework%20(Release).json)
* For detailed API documentation, please refer [API Docs](https://documenter.getpostman.com/view/6369926/TVRoZ6jW)

#### Deploy

If you would like to integrate with any mobile or web application, use [Ngrok](https://ngrok.com/download) to get a public URL of 
your localhost. Also, you can host in any of the online cloud service providers like [Heruko](https://www.heroku.com/), [Azure](https://azure.microsoft.com/), [AWS](https://aws.amazon.com/), etc.

## Community

Zinger framework is completely free and made open-source. Our team is really happy to support contributors from all around the world. Fork our project and send us your pull request: maybe sample mobile apps using our framework, minor extensions or major improvements.

**Every contribution is awesome and welcome!**
