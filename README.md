# MC (Midnight Commander)
Midnight Commander is a TUI (Text User interface) based console file management utility.

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
(Note: this command grants access to the current directory on your local filesystem to the 'mc' application running in the container)

## Help
`$ docker run -it --rm macabees/mc --help`
