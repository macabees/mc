# MC (Midnight Commander)
A TUI (Text User interface) file management utility. Makes managing files easier then remember all the commands.

## mc (Project Info)
[Website](https://midnight-commander.org/)

## Docker Hub
[Website](https://hub.docker.com/r/macabees/mc/)

## Build image
`$ docker build -t macabees/mc:latest .`

## Docker Push
`$ docker push -t macabees/mc:latest`

Note: requires `docker login`

## Run image
`$ docker run -it --rm --name mc macabees/mc`
(Runs the application in the isolation of the container [no external access to the local filesystem])

`$ docker run -it --rm -v $(pwd):/home/root --name mc macabees/mc`
(Note: This version of the command grants access to the current directory on your local to the MC application)

## Help
`$ docker run -it --rm macabees/mc --help`
