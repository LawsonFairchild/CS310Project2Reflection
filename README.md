The purpose of the project is to deploy a containerized web app that can be accessed on another computer. 

The first task was to install sudo on to the computers. The required that we access the internet. It allowed us to run commands as root even if we weren't logged in as root. 
The second task was to set up the computer so that it could be ssh-ed into and set up a shortcut in csa to ssh into it more easily.
The third task was to set up a simple web app that can be accessed on another computer.
The fourth task was to set up flask as a container that can run on another computer.

One hurdle we ran into was that we put the wrong IP address when connecting to the internet. It actually worked, but it caused problems in the future. It was a simple fix once we figured out the problem. We just changed /etc/network/interfaces so reflect the proper IP address.
Another hurdle we ran into was that for some reason Docker decided to uninstall itself so we had to reinstall it.
A third hurdle we hit was that when setting up taiga, we told it to search for the files on the local machine. This caused an error when we tried to open it on another computer. We just changed the file telling it to search locally to 10.0.154.6 (our server's IP).

If I were to redo this project, I would research docker more first and make sure I understood what was going on before I tried to use it. I would also double check the IP address before closing the file.

I think it would be helpful to combine steps 3 and 4 together (but still give us the same amount of time). I think it would be helpful to do things all at one time since by the time we get around to the 4th step, I've already forgotten certain things about step 3. 
