# Microservice Architecture in ASP.NET Core with Ocelot API Gateway

Let's Learn Microservice Architecture in ASP.NET Core with API Gateway!

We'll go through a popular way of Building Applications – Microservice Architecture in ASP.NET Core. In this detailed article, we will try understand what really Microservice architecture is? , How does it compare to the traditional way of building application? And also some advanced concepts like API Gateways with Ocelot, Unifying several Microservices, Health Checks and much more.

We will be building a Simple Microservice Application for demonstrating various Concepts including Microservice Architecture in ASP.NET Core, API Gateways, Ocelot, Ocelot Configuration , Routing and much more.

Read the entire Blog Post here - https://www.codewithmukesh.com/blog/microservice-architecture-in-aspnet-core/

# Steps

1. Create two DB
  a. customer2020 (From Microservice\Customer.Microservice\appsetting.json "DefaultConnection")
  b. product2020(From Microservice\Product.Microservice\appsetting.json "DefaultConnection")
2. In Visual Studio, Server Explorer\Data Connection, Add connection to the db and Test Connection for each DB
  Server Name: localhost\SQLEXPRESS  
  Database: customer2020  (Repeat for db product2020)  
  Credential: sa/Pk3G@cjN085U  

3. In Advance, copy connection string and update the following
  a. Microservice\Customer.Microservice\appsetting.json "DefaultConnection"
  b. Microservice\Product.Microservice\appsetting.json "DefaultConnection")
4. Right click solution\properties\Common Properties\Startup Project, select Multiple starup projects, and set all Action to start.
5. Delete 'Migration' Folder if exists
6. Run migration  
  a. In Tools\Nuget Pakacge Manager\Package Manager Console  
  b. Select Default Project Microservice\Product.Microservice (Repeat for Default Project Microservice\Customer.Microservice)  
  c. Run  
      Add-Migration InitialCreate  
      Update-Database  
7. Hit F5 or Click Start to test  
