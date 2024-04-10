# nomad-meteor

This is a fun project I've made to start and purge nomad jobs based on the meteors that spawn and explode in meteors. The game itself is an output of the[excellent tutorial of Miłosz Smółka](https://threedots.tech/post/making-games-in-go/).

## Excuses:
- Why do you have a monolythic main.go? It looks awful!

The main.go is the output of the tutorial. You write it as you go and end up with something like this at the end. If you want to see the properly structured one, see the github repo of Miłosz which contains the nicely structured solution.
- Why are the nomad calls using web requests instead of the SDK?

The nomad calls should indeed use the SDK, but since the main reason for making this was learning and having fun, I have decided to use the HTTP endpoint with requests. I might actually change this at some point

## Starting up
You need to install and start a nomad agent in dev mode before starting the application with the standard go run main.go