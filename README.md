## Overview

A simple bit of code to demonstrate how to convert a JSON file received from a public api address and provide the data as a downloadable csv file.

## Opening an html file in WSL

I couldn't get the html file to open when typing the usual command in the terminal and I suspected this was because I was using WSL2 (Windows Subsystem for Linux). Below is a Stackoverflow question which tackles this issue.

Check out this question from [Stackoverflow](https://stackoverflow.com/questions/67814265/what-is-the-best-way-to-open-html-files-from-vscode-when-using-wsl)

Run a simple HTTP server with the following command:

cd path/to/your/file  
python3 -m http.server 3000

It is now possible to connect to the localhost in WSL at port 3000 from the Windows system via the browser. However, http://localhost:3000 will not work. We need to use the IP address which WSL assigns. This can be found by running the command 'ip route'
Select the IP address after link src as shown below.

Thus the IP address to enter into the browser and open the html file is:  
http://172.24.38.169/:3000/

![image](https://github.com/johnhm22/JSON-to-csv-download/assets/71333679/374e2a28-192f-41c4-8665-4cbf8c133f62)  


### Note  
More recently when this repo was cloned and tried out, it was discovered that a connection using http://localhost:3000 worked successfully as did the approach using the IP address obtained from the command 'ip route'.  

Alternatively the 'live server' extension for VS Code also works. Once installed, the server can be initiated by clicking on 'Go live' found in the right hand bottom corner of VS Code. 


![image](https://github.com/johnhm22/JSON-to-csv-download/assets/71333679/c6ed035d-7aba-4e0c-9aef-00f51fbb968e)


Live server provides the address http://localhost:5500/ as can be seen below:  

![image](https://github.com/johnhm22/JSON-to-csv-download/assets/71333679/c08aa913-97b7-42fc-b431-8a4b8c8b59d7)  


Another method to start the server is to right-click on the html file to bring up menus and select 'Open with Live Server'.  

![image](https://github.com/johnhm22/JSON-to-csv-download/assets/71333679/3c5e9976-f459-454d-87d6-2913f3281d4b)




## Reference

Credit to [OpenJavaScript](https://www.youtube.com/watch?v=JPxzeG4N5nQ)
