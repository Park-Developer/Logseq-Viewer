# Logseq_Viewer
 - Version : V1.0
 - Date : 26.01.02
 - Created by Daniel Park
 
<p align="left">
 <img width="80" height="60" src="Image/icon.png">

</p>
<br>

### *Introduction*

I think Logseq is awesome free tool to manage todo lists or daily notes. However, It is hard to manage all tasks effectively if I only use Logseq. So, I decided to make a viewer program to visually manage all tasks written in Logseq. 

<br>

### *Concept*

Logseq Task Management Program to visualize task lists and their respective statuses

<br>

### *How to use?*

1. You must create logseq.json in the Logseq folder.
<p align="center">
 <img width="460" height="300" src="Image/image.png">

</p>


2. Input your Logseq folder address in the "Logseq_Address" in logseq.json

    ```json
     {   
     "INFO" : {
         "Description":"Logseq setting file for execution",
         "Version": "Logseq Viewer V1.0",
         "Notice":"You must input Logseq folder directory. Otherwise the viewer file will not be created"
     },
     
     "SETTING":{
         "Logseq_Address" : "C:\\Users\\gnvid\\OneDrive\\바탕 화면\\logseq",
         "Mode":"RUN",
         "Style":"TBD",
         "Calander Range":"TBD"
     }
     }
    ```

    - Logseq_Address : Directory of Logseq folder
    - Mode "RUN" : Create logseq_view.html automatically 

3. You can set debugging mode in the main.py file

   ``` Python
   ''' [DEVELOPER SETTING] '''
 
   DEBUG_MODE=True # True : Debugging Mode
   ```

<br>

### *Function*
 - Visualization
 - Task Filtering
 - Priority Filtering
 - Assignee Filtering  
 - Period Change
 
<br>

### *Installation*
```bash
pyinstaller -w -F --icon=Image\icon.ico -n logViewer main.py
```

