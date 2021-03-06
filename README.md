# webppl-agents
Webppl library with agents for solving MDPs and POMDPs. JS library for displaying Gridworld. 

#Running script in browser

Running a webppl script in the browser allows use of `GridWorld.draw` for easier debugging of agents. To do so, do we first have to install webppl from source and link it to node. 

This clones webppl into the directory above yours and links it to the global node webppl installation.

If `npm link` doesn't work due to permissions, you can use sudo or [follow this](http://justjs.com/posts/npm-link-developing-your-own-npm-modules-without-tears). 

```
sh install.sh
```

Then we can compile webppl and webppl-gridworld together and run your script.

```
sh compile.sh examples/hyperbolic/generative_examples.wppl
```

To just run your script without compiling we can do. 

```
sh run.sh myscript.webppl
```


To run purely on the command line we need to install some webppl packages:

```
mkdir ~/.webppl
npm install --prefix ~/.webppl https://github.com/stuhlmueller/webppl-dp
npm install --prefix ~/.webppl https://github.com/stuhlmueller/webppl-timeit
npm install --prefix ~/.webppl https://github.com/stuhlmueller/webppl-viz
```
