# Networking-setup
Task Description: Task 13	"🔰 Create a Setup so that you can ping google but not able to ping Facebook from same system"

Problem Solution:
Step 1) First of all run command "route -n" , it will show that you have  a gateway , using which we can go to public internet.

![Capture1](https://user-images.githubusercontent.com/50879814/114296858-18cc1a80-9acb-11eb-8494-96775b857aad.PNG)

Step 2) Run Command "nslookup www.google.com" , it will show one of the IP of google server.

![Capture2](https://user-images.githubusercontent.com/50879814/114296921-6cd6ff00-9acb-11eb-846b-3e5debfd21d2.PNG)


Step 3)We can ping to that ip of google.





![capture3](https://user-images.githubusercontent.com/50879814/114296952-9db73400-9acb-11eb-91bb-625916daf232.PNG)

Step 4) Similary do nslookup "www.facebook.com" , to see one of the ip of facebook server and we can ping to that ip of facebook server also.

![Capture4](https://user-images.githubusercontent.com/50879814/114297010-ea9b0a80-9acb-11eb-9a52-da5ed6ac8733.PNG)

Step 5) Now , we can delete the router gateway by "route del -net 0.0.0.0" command , after this we cann't ping to any of the ip of public world (i.e we cannot ping to google and facebook also)

![Capture5](https://user-images.githubusercontent.com/50879814/114297098-5bdabd80-9acc-11eb-948c-514590aad8d2.PNG)

Step 6) Now , we can add a route so that we can ping to google but , we cannot ping to facebook.

![Capture6](https://user-images.githubusercontent.com/50879814/114297135-8c225c00-9acc-11eb-8da8-358066d6d64b.PNG)

The required task is solved now 
![Capture7](https://user-images.githubusercontent.com/50879814/114297167-b4aa5600-9acc-11eb-8e4a-4bff54eddc1c.PNG)






