Raspberry Pi mini monitoring tool
==============

After trying some monitoring tools like Cacti or Nagios on my 1st gen Raspberry Pi, and seeing that either they used too 
many resources or had too many options I wouldn't use, I decided to develop a really simple dashboard that would show 
some system stats.

Right now it's just showing the CPU load and temperature and the memory usage.

It's just HTML plus the dygraphs JavaScript Visualization Library (http://dygraphs) which is used to display the charts.

You can see the live stats of my Raspi at http://stats.ariste.info.


**Requisites**
* bc: Basic Calculator used in the temperature script to obtain decimal values.


**Installation**

1. Copy the content of the html folder to the root directory of your web server.
2. Copy the content of the script folder to /usr/bin or any other of your choice.
3. Edit your crontab. There's some examples in the crontab.txt file for help.
4. Wait some time so the scripts create the logs.
5. Point your browser to the location of index.html.
6. That's all, it should run.


**TO-DO's**

- Think about using a SQLite database instead of logs.
- Let the user choose the period of time to be displayed.

contact: adria@ariste.info
