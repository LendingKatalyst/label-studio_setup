# Update 

We can create a shortcut on the desktop that opens up the anaconda prompt and enters the following cmds that will open the label studio platform on the browser. 

Resource : https://stackoverflow.com/questions/60290516/automatically-execute-commands-on-anaconda-prompt-startup



Open Anaconda prompt (anaconda3) by searching in the seach bar at the bottom : 


# Entering manual commands (Alternative)

Make sure (base) is visible on the left end:

Step 01 :
```
conda activate label-studio
```

(label-studio) will be  visible to the left in place of (base)


Step 02 : enter the following command
```
set LABEL_STUDIO_LOCAL_FILES_SERVING_ENABLED=true
```

Step 03 : enter the following command 
```
set LOCAL_FILES_DOCUMENT_ROOT=C:\Users\kiran\Desktop\expt01
```


Step 04 : enter the following command, a mozilla window should open displaying  label studio projects
 ```
 label-studio start
 ```
 
 Step 05 : If mozilla firefox does not open,  please wait for some time and do the following 
 
 Open the mozilla browser and enter the following address which takes you to the label-studio interface
 ```
 http://0.0.0.0:8080/projects/
 ```

Step  06: 
IMPORTANT !!!
Make sure you logged into the correct accound if not please log out and enter your credentials . 
