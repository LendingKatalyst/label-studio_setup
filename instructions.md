Open the terminal(Right click --> open terminal) : 

Make sure (base) is visible on the left :

Step 01 :
```
conda activate label-studio
```

>> Once (label-studio) is visible to the left in place of (base)


Step 02 : enter the following command
```
export LABEL_STUDIO_LOCAL_FILES_SERVING_ENABLED=true
```

Step 03 : enter the following command : an output "true" should be printed after that .
```
echo $LABEL_STUDIO_LOCAL_FILES_SERVING_ENABLED
```

Step 04 : 
 ```
 label-studio
 ```
 
 Step 05 : 
 
 Open the mozilla browser and enter the following address which takes you to the label-studio interface
 ```
 http://0.0.0.0:8080/projects/
 ```

Step  06: 
IMPORTANT !!!
Make sure you logged into the correct accound if not please log out and enter your credentials . 
