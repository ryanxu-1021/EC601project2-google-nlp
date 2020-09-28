# EC601project2-google-nlp 
Jiachen Xu   email:ryanxu@bu.edu

I actually have some problem with the venv which is set up to isolate dependencies. I can't install the google cloud language or google cloud storage in that virtual environment.
So I just do it in the normal directory.

The first thing to do is installing the client library.
<img src="1601261078(1).png">
Then setting up authentication.
<img src="1601261119(2).png">
And I need to using powershell behind a proxy server.
<img src="1601261195(3).png">
Then I run the example shown in the Using client library, it works.
<img src="1601261246(4).png">
Then I combine the function of entities and sentiment together.
I input the following text, LAKERS OR HEAT? LeBron James faces off with former coach Erik Spoelstra in the #2020NBAFinals.
There is the result
<img src="1601261394(5).png">
<img src="1601261453(6).png">
It can recognize the name for example, Lebron James and Erik Spoelstra and also give the link of wikipedia. And it can also recognize the team such as LAKERS, but HEAT can
 not be recognized. I think it's because there are many different other meanings of heat. And the system may be not good enough to analyze its actual meaning.
