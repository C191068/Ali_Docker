# Intro

![Screenshot from 2023-11-10 12-16-25](https://github.com/C191068/Ali_Docker/assets/89090776/5fcc976d-a142-4444-9891-f56ff08ac010)
![Screenshot from 2023-11-10 12-18-27](https://github.com/C191068/Ali_Docker/assets/89090776/343140cd-7cc0-4bbb-a354-37c143af547d)
![Screenshot from 2023-11-10 12-20-15](https://github.com/C191068/Ali_Docker/assets/89090776/6faa03fa-2395-46e0-af2f-17fd21bd41f4)

Monolethic archutect are build on a single unit <br>
it means an IDE will hold ultile projects and will be comile in a single unit <br>

they are also deployed as a single unit <br>

they are dulicated on each server <br>

it means if we hd to scale the system we have to spin the new VM <br>

and copy and delpoy the whole system on VM <br>

![Screenshot from 2023-11-10 14-14-09](https://github.com/C191068/Ali_Docker/assets/89090776/9f853290-49a3-4cad-9538-007ec1d7fdb1)

examle is 3 tier application <br>

even though the system was separated into layers iut was tighty coupled from the web project <br>
 to the business layer project <br>

 and the whole system will run in same address space <br>

 with microswervies we break our big sytem into smaller parts <br>

 each wit its own responsibility <br>

 
let us say we have a class that deal with idenity with business layer <br>

we can extract that code and place it in own mcroservice <br>

we can then scale each of these smaller pieces indeendently from each other <br>

there is no srong bound since we exose functionality through AI <br>

they can be written by smaller teams nd each can use their own <br>

programming languages like Go, PHP and C# <br>

domain specific data can be stored in separate dataases <br>

![Screenshot from 2023-11-10 14-31-05](https://github.com/C191068/Ali_Docker/assets/89090776/131d9333-24e9-4f3d-b1aa-826f77c8694d)


the way we will deploy a monolithic system  is by deloying everything on a server <br>

![Screenshot from 2023-11-10 14-33-54](https://github.com/C191068/Ali_Docker/assets/89090776/7326ac1c-0baf-41c6-b905-cd388c4565f3)

we have to scale and deploy everything on more servers <br>


microservices are deloyed indeendently <br>

![Screenshot from 2023-11-10 14-36-23](https://github.com/C191068/Ali_Docker/assets/89090776/f0205911-399f-4367-8df7-0d6fb9904778)

they can be scaled independently also <br>


how can we convert monolithic system to icroservice architecture <br>

we need to break it into small units <br>

unlike the code that dealt with ientiy in busines layer <br>


Martin fowler author author of atterns of entrrise applice architecture <br>

book documented a way to achieve such transformation <br>

using yhe strangler pattern <br>


# Micrservoces anti pattern <br>



from one monolithic system if we handle a bunch of small pieces there is a risk of unnecessary <br>
complexities <br>

a change in microservice can take our system down <br>

securing all mcroservices is not so easy <br>

# Microservice benefits <br>

since each microservice runs at its own adress space <br>

there are less chances if one of them goes the whole system will go down <br>


a microservice runs on open source technologies <br>














 
