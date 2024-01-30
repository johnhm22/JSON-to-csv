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

![image]/home/johnm/code/src/github.com/johnm/JSON-to-csv/Images/IP_address.jpg

Thus the IP address to enter into the browser and open the html file is:  
http://172.31.98.33:3000/

## Reference

Credit to [OpenJavaScript](https://www.youtube.com/watch?v=JPxzeG4N5nQ)
