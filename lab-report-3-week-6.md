# Lab Report 3 Week 6
Andy Liu, A171112518

## Streamlining ssh Configuration

![Image](img3/opening-config-file.PNG)

First, type in 
```
 ~/.ssh/config
 ```
  to open up the config file. If it does not exist, it can be created in vscode.
```
  cd ~/.ssh 

  code .
  ```

  The first line of code will enter you into the ssh directory. The second line of code will open the folder up in vscode. From there, you can just click new file.

![Image](img3/ssh-config-file.PNG)

  Inside the file add this: 
  ```
  Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lwi22aiv
  ```

  I get to choose what comes after "Host" on the first line. The HostName has to be thename of the server, and the User has to be my username.

![Image](img3/ssh-ieng6.PNG)

Now, I can log into my ieng6 account with just
```
ssh ieng6
```

![Image](img3/scp-week-6.PNG)

Now, I can scp using 
```
// scp filename config
scp lab-report-3-week-6.md ieng6
```
