# How to contribute?

Our goal is build an application that some one who is moving or even selling things can easily configure it.
You can see or open issues [here](https://github.com/anapaulagomes/to-vendendo/issues). If you have any doubts please say hi at [gitter](https://gitter.im/to-vendendo/Lobby).

## Steps

Steps to contribute:

1. Look for a issue or open a new one [here](https://github.com/anapaulagomes/to-vendendo/issues) or just drop by on our [gitter](https://gitter.im/to-vendendo/Lobby)
2. Create a new branch with an intuitive name (thinking about the concept of [feature branch](https://martinfowler.com/bliki/FeatureBranch.html)
3. Do amazing stuff and have fun
4. Run tests
5. If they are passing, you are free to commit and push
6. Open a Pull Request with a description and the issue reference

Test-Driven Development is awesome to thinking about the design first and keep things simples. We recommend it.

## Best Pratices

Let's try to keep the code as simple and clean as we can. Some good pratices to follow during the contributing process:

- **Respect the PEP8**: don't forget to check the PEP8 complains; you can use pre-commit hook to help you with
- **Write Tests**: **always** write tests for your code
- **Use Feature Branch**: if you are fixing a bug, please add `hotfix/branch-name` to your branch name; if is a feature, add `feature/branch-name`
- **Keep the Cordiality**: be polite and kind; words like please and thank you are welcome :)

## Configuration

To run the code you need `Postgres 9.6` and `Python 3.6`. After that, in the repository folder execute:

`make setup`

We recommend to use virtual environments like [virtualenv](https://virtualenv.pypa.io/en/stable/) or [pipenv](https://docs.pipenv.org/).

- Docker

_Available soon_

## Troubleshooting

- Database is not running

```
E         sqlalchemy.exc.OperationalError: (psycopg2.OperationalError) could not connect to server: Connection refused
E       	Is the server running on host "127.0.0.1" and accepting
E       	TCP/IP connections on port 5432?
```

- Database was not created

`sqlalchemy.exc.OperationalError: (psycopg2.OperationalError) FATAL:  database "tovendendo_test" does not exist`
