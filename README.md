# Intro

![Screenshot from 2023-11-10 12-16-25](https://github.com/C191068/Ali_Docker/assets/89090776/5fcc976d-a142-4444-9891-f56ff08ac010)
![Screenshot from 2023-11-10 12-18-27](https://github.com/C191068/Ali_Docker/assets/89090776/343140cd-7cc0-4bbb-a354-37c143af547d)
![Screenshot from 2023-11-10 12-20-15](https://github.com/C191068/Ali_Docker/assets/89090776/6faa03fa-2395-46e0-af2f-17fd21bd41f4)

Monolethic archutect are build on a single unit <br>
it means an IDE will hold multiple projects and will be compile in a single unit <br>

they are also deployed as a single unit <br>

they are dulicated on each server <br>

it means if we had to scale the system we have to spin the new VM <br>

and copy and delpoy the whole system on VM <br>

![Screenshot from 2023-11-10 14-14-09](https://github.com/C191068/Ali_Docker/assets/89090776/9f853290-49a3-4cad-9538-007ec1d7fdb1)

examle is 3 tier application <br>

even though the system was separated into layers it was tighty coupled from the web project <br>
 to the business layer project <br>

 and the whole system will run in same address space <br>

 with microswervies we break our big sytem into smaller parts <br>

 each wit its own responsibility <br>

 
let us say we have a class that deal with idenity with business layer <br>

we can extract that code and place it in own microservice <br>

we can then scale each of these smaller pieces independently from each other <br>

there is no strong bound since we expose functionality through API <br>

they can be written by smaller teams and each can use their own <br>

programming languages like Go, PHP and C# <br>

domain specific data can be stored in separate dataases <br>

![Screenshot from 2023-11-10 14-31-05](https://github.com/C191068/Ali_Docker/assets/89090776/131d9333-24e9-4f3d-b1aa-826f77c8694d)


the way we will deploy a monolithic system  is by deloying everything on a server <br>

![Screenshot from 2023-11-10 14-33-54](https://github.com/C191068/Ali_Docker/assets/89090776/7326ac1c-0baf-41c6-b905-cd388c4565f3)

we have to scale and deploy everything on more servers <br>


microservices are deloyed independently <br>

![Screenshot from 2023-11-10 14-36-23](https://github.com/C191068/Ali_Docker/assets/89090776/f0205911-399f-4367-8df7-0d6fb9904778)

they can be scaled independently also <br>


how can we convert monolithic system to microservice architecture <br>

we need to break it into small units <br>

unlike the code that dealt with identity in busines layer <br>


Martin fowler author author of patterns of enterprise application architecture <br>

book documented a way to achieve such transformation <br>

using the strangler pattern <br>


# Micrservoces anti pattern <br>



from one monolithic system if we handle a bunch of small pieces there is a risk of unnecessary <br>
complexities <br>

a change in microservice can take our system down <br>

securing all mcroservices is not so easy <br>

# Microservice benefits <br>

since each microservice runs at its own adress space <br>

there are less chances if one of them goes the whole system will go down <br>


a microservice runs on open source technologies <br>

so there is a less vendor lock in <br>

since they are smaller they are easier to understand <br>


it makes them faster to deploy <br>

and easier to scale <br>

so we have to make sure that our team is well trained and has made <br>

some proof of concept and make sure to add one iece at a time  <br>

testing might appear simpler since there are less functionality <br>

in a microservice to test <br>


deployment may appear simpler <br>

we aready to manage multiple databases <br>

calls throug microservices will go through apis <br>

and this will add a bit of latency to all calls <br>

so we make sure we test for that <br>

trnsient error means if we make a call it will fail <br>

but if we try again 59 milliseonds later and it will work <br>

so we will amke sure to imlemet some retry stategy to our code <br>

by using aservice mesh <br>

cloud native is away to build and architect comlex system <br>

taking dvantage of modern develoment practices <br>
and use of cloud infrastructure <br>

cloud ntive uses containers , service meshes , microservices ,immutable <br>
infrastructre <br>
and declarative apis <br>

immutable infrastucture mens we usually nevr udate something <br>

but we replace it with newer version <br>

Loosly couled system means functionalities are exosed through APIs <br>
obsevable with th use o metrics <br>

cretion and udates are autumated <br>

and instead of making changes once every six months <br>

we deloy eye impact changes on a frequent basis <br>


and finally we use a series of oen source projects to run our system <br>


![Screenshot from 2023-11-10 15-47-53](https://github.com/C191068/Ali_Docker/assets/89090776/27eb0f2c-7780-47b3-85eb-23dd0ee124a7)

the above cncf landscape graph shows a ton of open source projects <br>























 
