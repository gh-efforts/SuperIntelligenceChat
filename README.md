# SuperIntelligenceChat AI
# Background
In the modern data-driven business environment, the ability to acquire and analyze data is essential. However, for many non-technical people, SQL (Structured Query Language) writing and database operation are still a huge obstacle. Especially in a complex database system like Filecoin, it is extremely difficult and time-consuming for users without a technical background to find the required data location, write the correct query statement, and obtain accurate results.

We have developed an innovative tool designed to solve these problems. This tool uses AI technology to convert natural language queries into SQL queries, so that users do not need to master SQL writing knowledge or understand the specific details of data storage. They only need to enter their questions to get the required data results.

We will use the lily tool to synchronize Filecoin's data to the local database, and then connect Filecoin data through the AI ​​tool we developed.

This tool provides businesses and individual users with an easy, fast and efficient way to access and utilize data in the Filecoin database. By eliminating technical barriers to SQL writing and data storage, anyone can easily obtain the information they need, thereby significantly improving the convenience and efficiency of data use. This not only saves development time and costs, but also allows users to focus more on the value of the data itself and make smarter business decisions.
## Core advantages
1. Eliminate technical barriers

- Non-technical people no longer need to learn SQL language. This tool can understand the user's natural language query and automatically generate the corresponding SQL statement. For example, users only need to enter "What is the total number of votes that miner f0xxxxx won in the height range 4034428 to 4035229?", and the tool will automatically generate and execute the corresponding SQL query and return accurate results.
2. Transparent data storage:
- Users do not need to know where the data is stored in the Filecoin database. Our tool handles all database interactions, and users only need to focus on what data they need without worrying about how to find and extract this data.
3. Enhanced data access flexibility:
- Traditional data access methods usually require dedicated front-end pages and back-end interface development to meet specific business needs. This is not only time-consuming, but also increases development costs. Our tool completely eliminates these needs. Users can make queries at any time according to business needs without waiting for the development and deployment of customized pages.
4. Save time and resources:
- By eliminating the complex front-end and back-end development process, enterprises can significantly save time and resources. Non-technical personnel can immediately obtain the data required for the business and make quick and data-based decisions, thereby improving overall operational efficiency.
5. Solve the problem of accessing Filecoin data:
- Although the Filecoin browser provides some data query functions, users may not be able to find the right tools for some specific and complex queries. Our solution makes interaction with the Filecoin database simple and intuitive, allowing users to ask various queries at will and get detailed answers.
# Technology Architecture
![Technology Architecture](/resources/liliai.jpg)
1. First, we synchronize the data of the Filecoin chain to the local database through the Lily tool for storage, and synchronize in real time.
2. The table structure, the filecoin official documents, some commonly used document terms, commonly used query SQL, and questions are vectorized and stored together with the original data in a vector database.
3. When the user enters natural language, the user's input is vectorized, and then the correlation is matched in the vector database to find the DDL, documents, SQL, etc. with high correlation. Then, these data and the user's questions are assembled into a prompt project for a large model query, and then the large model is called for reasoning and returning SQL. The program uses the generated SQL to query data and return data.
4. Then, the returned query data is combined with the user's questions and related documents to build a prompt project for generating BI icons again, and the large model is called to return the code for generating BI charts. So that the icon is displayed on the page.
5. If the generated SQL meets your requirements, you can also click the approval button to feedback the SQL to the training data, which can improve the accuracy of SQL.
# Demo
 Coming soon...

