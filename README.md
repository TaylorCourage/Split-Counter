# Split Counter

Admittedly not the greatest name out there for a website, but it does the job.

## What it is

This is a *very* basic webpage I threw together to help myself, and my co-workers out at my day job as a wiredraw machine operator. Often times customer requirements state that a coil of steel needs to have a specific maximum weight - typically less than we normally ship out - an accurately eye-balling where the midway point of several kilometers of steel is quite difficult. Instead of trying to guess where this point is, and shipping out products that could potentially be outside of customer specfications, we can accurately calculate this point and use that in conjunction with hardware installed on the machines to ship a quality product, every time.

## How it works

When a machine operator happens upon an order that requires the raw coil to be split, they will enter the asked-for details on the webpage, which will give them several different values to be used on the machine counter. For example, if the operator on machine 22 has an order that is to be drawn down to a finish size of 0.320" with a rack weight of 2,100lbs, they will enter those details (along with the diameter of the finish block), which will give the operator three values, one of which will be associated with the counter on the machine (either feet, inches, or rotations of the block).

## How to deploy

The goal of this project was to make it as simple as possible to implement. By using inline scripts and styles, and no external dependencies or files, you don't need an internet connection, or even a web server to use it - you can simply open the `.html` file in any modern browser (that supports JavaScript), on any modern platform, and get to work. This makes it easy to deploy to devices in facilities where there is weak, or no internet connection. This single-file nature also makes it very easy to deploy from virtually any web server (that supports JavaScript). You can test out my implementation available at https://splitter.taylorcourage.net, which is running on Nginx.

## Can I adapt this to my wiremill/other project?

Absolutely! This is why I have uploaded the code here for anyone to download, modify, and run as you please. The current implementation is designed for wiremills that operate in inches, but modification to metric should be possible. If you do not have the capability to modify this code yourself to match your facility, please get in touch and we can work something out (I'm available for hire as a developer!).