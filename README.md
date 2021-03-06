# Books and Authors 
This project is for demonstration purpose to verify the performance/how quick the data of 20k records can be retrieved using EntityFramework / Elastic Search

![image](https://user-images.githubusercontent.com/5477822/163704745-fb493ee1-899a-4050-adc9-f12a2f50d659.png)

# Description	
This project is done using Code-First approach in Entity Framework, Create two tables i.e Book and Author
- Create a many to many relationships between Book and Author
- When application launches first time and there is no data in database, seed (insert) 20,000 records for books and each book should be tagged at least to i.e 2 authors randomly
 
<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/5477822/163707722-6d7c7958-24ad-485f-b336-ee04efba666d.png">
</p>

- Listing screen of Books with server-side pagination and fetch the data using EF via LINQ & ElasticSearch
- Search by Books and Authors with a delay of 300ms through EF and Elastic
- Print button which prints the entire grid (with no style) and View button to open PDF in new tab


# Built With
	1. ASP.NET WEBAPI
	2. Entity Framework
	3. SQL
	4. AutoMapper
	5. Angular
	6. ElasticSearch
	7. Bootstrap

# Prerequisites
Below was the list of software’s required to run this application 
 
1.	Visual Stuido Code – Angular latest (to run web application)
https://angular.io/guide/setup-local
https://www.c-sharpcorner.com/article/how-to-install-angular/
2.	Visual Studio 2019 or version supports .Net framework 4.6.1 3. 
3.	Elastic Search (https://www.elastic.co/elasticsearch/)

	Installation: - 
	1. Download the Zip file and extract, add the bin path to Path variable under system variable
	2. Open the command prompt and run the command **elasticsearch** wait for the command to run 
	3. Open the browser https://localhost:9200/ or http://localhost:9200/ (Disable the security in elasticsearch.yml if not required- eg : C:\elasticsearch 8.1.2\config\elasticsearch.yml)


# How to run this application
1.	Clone the repo or download     git clone https://github.com/jagadeesh-dotnet/AngularWebAPIEntityandElastic.git
2.	**Restore Nuget packages** for WEBAPI project - AngularAspNetAPIElasticsearch
3.	Run **npm install** for WEB project to restore packages - BooksWeb
4.	Before running the applications check/modify the web.config (eg: elastic password,  url etc.,)
5.	Make sure the elastic search is running
6.	Run the application which seeds the 20k records (sample data) in SQL and Elastic Search (It takes around 2minutes)
7.	Now run the web application

![image](https://user-images.githubusercontent.com/5477822/163706110-10a0bab7-eddc-498a-8035-c7d01a5d5291.png)
