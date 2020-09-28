# EC601project2-google-nlp 
Jiachen Xu   email:ryanxu@bu.edu

I actually have some problem with the venv which is set up to isolate dependencies. I can't install the google cloud language or google cloud storage in that virtual environment.
So I just do it in the normal directory.

The first thing to do is installing the client library.

<img src="1601261078(1).png">

Then setting up authentication.

<img src="1601261119(2).png">

And I need to using powershell behind a proxy server. Or it will be working so slow that may take more than 10 minutes, and then the powershell will report an error.

<img src="1601261195(3).png">

Then I run the example shown in the Using client library, it works. It just input the text "Hello World!", and analyze its sentiment. The result shows it's a positive sentence.

<img src="1601261246(4).png">

I want to use more functions of NLP and want to analyze the text that I'm interested in. So I combine the function of entities and sentiment together.

I input the following text, LAKERS OR HEAT? LeBron James faces off with former coach Erik Spoelstra in the #2020NBAFinals.

I want to see whether it can exactly tell what LAKERS and HEAT are and so as the names. 

There is the result

<img src="1601261394(5).png">

<img src="1601261453(6).png">

It can recognize the names. The system recogenizes Lebron James and Erik Spoelstra. They are also given the link of wikipedia. And it can also recognize the team such as LAKERS, but HEAT can not be recognized. I think it's because there are many different other meanings of heat. And the system may be not good enough to analyze its actual meaning. As for the sentiment, the Google nlp thinks it's a kind of negitive sentence.
