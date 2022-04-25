# DevOps Exercise

This project is meant to test skills for the VoteShield DevOps Engineer role. What it does is not that important.

See [./INSTRUCTIONS.md](./INSTRUCTIONS.md) to get started.

## Usage

This exercise provides a "thing" REST API.

- `/things`: List all things
- `/things/<id>`: List specific thing

## Install

- Install with [poetry](https://python-poetry.org/)

## Development

- Run `python app/main.py`

## Deployment

Docker file provided so first we build image with these instructions
and run docker image with exposed port 5000 to host machine

```local sh
git clone Voteshield/devops-exercise.git
cd devops-exercise
docker build -t devops-excercise .
docker run -p 5000:5000 -it devops-excercise
```

Or, run docker-compose file and get same result

```local sh
git clone seru1us/devops-exercise
cd devops-exercise
docker-compose up
```

## Testing

- Run `python tests.py`

## Credits

- Inspiration from [bregman-arie/devops-exercises](https://github.com/bregman-arie/devops-exercises)