
[link](https://github.com/h586613/dat250-jpa-tutorial)

* **Technical problems that you encountered during installation and use of Java Persistence Architecture (JPA) and how you resolved them:**
<br>nothing being persisted:
<img width="408" alt="Skjermbilde 2023-09-17 kl  23 25 40" src="https://github.com/h586613/a1dat250/assets/54099085/653dad23-ebeb-4a61-81d0-ccab656dff40">

<img width="223" alt="Skjermbilde 2023-09-17 kl  23 25 30" src="https://github.com/h586613/a1dat250/assets/54099085/d69be00b-34e4-4e8a-bef3-660ec0d6263a">

* **An explanation of how you inspected the database tables:**
  persistance view -> ERD
<img width="190" alt="Skjermbilde 2023-09-17 kl  23 50 59" src="https://github.com/h586613/a1dat250/assets/54099085/afdfbc97-1880-4f30-95e1-dec00a9342f3">


* **what tables were created, screenshots:**

<img width="553" alt="Skjermbilde 2023-09-17 kl  21 58 50" src="https://github.com/h586613/a1dat250/assets/54099085/88b1aef1-fc9c-4b14-b87b-604d2da7bcbb">
<img width="535" alt="Skjermbilde 2023-09-17 kl  21 59 51" src="https://github.com/h586613/a1dat250/assets/54099085/8793b8f7-a540-4cfc-a104-25be6b278142">

<img width="559" alt="Skjermbilde 2023-09-17 kl  21 59 24" src="https://github.com/h586613/a1dat250/assets/54099085/9bd7b6b1-0534-469d-b936-9efdd5a7f078">



  <img width="375" alt="Skjermbilde 2023-09-17 kl  20 15 46" src="https://github.com/h586613/a1dat250/assets/54099085/edad814e-5731-4ae6-9759-cc2c4f765728">
<img width="234" alt="Skjermbilde 2023-09-17 kl  20 18 28" src="https://github.com/h586613/a1dat250/assets/54099085/b46517a4-d2f4-482e-819e-1c92fad1a6cd"> was stopped because of lack of credentials <br> <br>


Questions:

**Where is the database? Explain the used database and how/when it runs.** 
<br>when we look at persistence.xml we can see that:
* the database is located at this url:
  <img width="490" alt="Skjermbilde 2023-09-17 kl  20 21 55" src="https://github.com/h586613/a1dat250/assets/54099085/b29c5987-7e22-4a5a-a402-3fff0caaa114">


**Can you provide the SQL used to create the table Customer (Hint: Hibernate is used for the object-relational-mapping)?**
<img width="529" alt="Skjermbilde 2023-09-17 kl  20 22 48" src="https://github.com/h586613/a1dat250/assets/54099085/c4ad241c-d068-410b-bca7-96a119985135">
```
Hibernate: 
    create table Customer (
        id bigint generated by default as identity,
        name varchar(255),
        primary key (id)
    )
```


**Find a way to inspect the database tables being created and attach a screenshot of the database schema to your report. Do the created tables correspond to your initial thoughts regarding the exercise?**

see above. yes, the tables corresponded to my expectations after learning about how different relations are represented.

