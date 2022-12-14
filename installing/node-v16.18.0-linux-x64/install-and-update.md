# How to install/update

If you want to dive deeper into the Angular CLI and learn more about its usage, have a look at its official documentation: https://github.com/angular/angular-cli/wiki

You encountered issues during the installation of the CLI or setup of a new Angular project?

A lot of problems are solved by making sure you're using the latest version of NodeJS, npm and the CLI itself.

## Updates: 

### Updating NodeJS:

Go to nodejs.org and download the latest version - uninstall (all) installed versions on your machine first.


### Updating npm:
```
sudo npm install -g npm
``` 
<sub>(sudo  is only required on Mac/ Linux)</sub>

### Updating the CLI
```
sudo npm uninstall -g angular-cli @angular/cli 
npm cache verify
sudo npm install -g @angular/cli 
```

## Common issues & solutions:
- Creation of a new project takes forever (longer than 3 minutes)
    - That happens on Windows from time to time => Try running the command line as administrator
- You get an EADDR error (Address already in use)
    - You might already have another ng serve process running - make sure to quit that or use ng serve --port ANOTHERPORT  to serve your project on a new port
- My changes are not reflected in the browser (App is not compiling)
    - Check if the window running ng serve  displays an error. If that's not the case, make sure you're using the latest CLI version and try restarting your CLI

