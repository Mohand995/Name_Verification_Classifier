# Name_Verification_Model


a-How to build the docker image? 

it's very simple as after pulling the image which it's link in the attachment it's only required to generate a running container of the image by running 

the following command (docker pull quay.io/mohand99/nameclassifier) 

b-How to test the solution?

provided in the repo file named Test_API.py that run two unit tests to test the api

you can find it on one of both:

http://127.0.0.1:5000/

http://172.17.0.3:5000/

after running the preceding command server link will be generated (http://127.0.0.1:5000/Guess_Name_DL  or  http://127.0.0.1:5000/Guess_Name_RF )  

you can send a request by curl command or postman with json body of the name you want to feed to the model

Note: sample of the request attached on the results folder in the attachment 

Note: in the modeling phase i have developed two models:

1-Random forrest model which works very well with low inference time can be accessed by the following endpoint [ http://127.0.0.1:5000/Guess_Name_RF]

2-Deep NN developed from scratch can be accessed by the following endpoint [http://127.0.0.1:5000/Guess_Name_DL]

c-How to verify the claim?

the results attached in result folder for the both endpoints would be enough to verify that both the models solve the problem in a good manner.


Correct Name :

![alt text](https://github.com/Mohand995/Digified_task/raw/master/Results/Correct/RF_MODEL2.jpg?raw=true)


Fake Name: 

![alt text](https://github.com/Mohand995/Digified_task/raw/master/Results/Fake/RF_Model1.jpg?raw=True)
