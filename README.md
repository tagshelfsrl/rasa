# Rasa (Tagshelf Version)

Rasa is an open source machine learning framework to automate text-and voice-based conversations. With Rasa, you can build chatbots on:
- Facebook Messenger
- Slack
- Microsoft Bot Framework
- Rocket.Chat
- Mattermost
- Telegram
- Twilio
- Your own custom conversational channels

or voice assistants as:
- Alexa Skills
- Google Home Actions

Rasa's primary purpose is to help you build contextual, layered
conversations with lots of back-and-forth. To have a real conversation,
you need to have some memory and build on things that were said earlier.
Rasa lets you do that in a scalable way.

## Breaking Changes from Original Repo

- Added new flag option `--remote-path` which allow us to specify the path of the remote storage independently of the local path.

### Code Style

To ensure a standardized code style we use the formatter [black](https://github.com/ambv/black).
To ensure our type annotations are correct we use the type checker [pytype](https://github.com/google/pytype). 
If your code is not formatted properly or doesn't type check, travis will fail to build.

#### Formatting

If you want to automatically format your code on every commit, you can use [pre-commit](https://pre-commit.com/).
Just install it via `pip install pre-commit` and execute `pre-commit install` in the root folder.
This will add a hook to the repository, which reformats files on every commit.

If you want to set it up manually, install black via `pip install -r requirements-dev.txt`.
To reformat files execute
```
make formatter
```

#### Type Checking

If you want to check types on the codebase, install `pytype` using `pip install -r requirements-dev.txt`.
To check the types execute
```
make types
```