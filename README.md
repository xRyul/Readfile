# Readfile

Dashboard to see the flow of images within photostudio environment.

When you run the script: ServerImageFlow.csv is generated on the ~/Desktop/ which then can be previewed with a SPACEBAR. 

It mostly works by reading simple CSV files, combining multiple outputs into 1, and then displaying the totals within the dashboard. Which then can be further processed and analysed to improve photostudio efficency as needed. 

<i> Originally I have created it to see where the images go missing. But later it evelved into something else. A tool which could be used by multiple studios and their managers - to locate not only where their images go missing, but also where their efficency could be improved.

It had to be something that used the tools readily available on (every) Mac System (no admin password, no ability to install 3rd party addons and tools), thus the reason for using simmple CSV, bash and Automator for image tracking. </i> 

![ReadFile-Dashboard Example](https://imgur.com/XBJLtmD.jpg)

---
## Main Benefits
- Ability to visualise missing images.
  - Images which didn't pass certain stage or department are automatically flagged, and show a RED icon 🛑 to indicate that there are issues and need users attention. Which allows for easy tracking and locating of the product in question. 
  - ![Flagged product shows red sign and requires users attention](https://imgur.com/I6VKr7o.jpg)
- Helps to visualise how many products and images are at any given moment in each department.
- Helps to build strategies and priorities based on volume.

### Other benefits
- Helps to visualise what to prioritise, and where are the bottlenecks. 
- Helps with any delays in delivery. 
- Helps with consistency of the photostudios production and flow. Checks how many exports were made by photographers and stylists. If 0, then you know that yuo would need to go and ask them to export.
- If certain targets are not met by X time, you can easily see **why** and **where**. 
---




# Dashboard has 3 main categories 
1. Production (Available to Retouch / Input). Which Consists of: Stylists & Photographers. Anything what was shot will show up here. That's the input. 
2. Work in Progress (WIP) - Images/ Products/ SKUs which Retouchers are currently working on
3. Output - total images which were uploaded to remote servers 

A quick summary is then generated at the very bottom of the dashboard: 
![Quick Summary with totals from each category](https://imgur.com/gJKcGHH.jpg)


### Why use CSV?
I had 2 options: .csv or .txt All other options were not always available on the mac by default. They either required admin password or 3rd party instal - 2hich was not an option. 

.txt - sometimes would lose formatting. 
.CSV - everyone had it. It stays nicely formated when you hit SPACEBAR. There is no need to open the file to view its contents. Which reduces the friction needed when all you want is to quickly glance who exported what. 


### Why switch to a ZSH?
SPEED! On ZSH, on average it runs 30s faster.
