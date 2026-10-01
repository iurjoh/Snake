# Snake starter repository

[Português (Brasil)](README.pt-BR.md)

## Idea and process

Despite its name, this repository currently contains the Code Institute Python terminal template, not an implemented Snake game. Source reviewed on 2026-10-01. `run.py` contains only comments and requirements.txt only a placeholder. No game loop, board, collision logic, planning record or design diary was found in the reviewed source.

## Architecture and design

The Node/Total.js wrapper serves a browser terminal and a raw WebSocket. `controllers/default.js` starts `python3 run.py` in an 80-column, 24-row pseudo-terminal for a connected client. index.js starts Total.js in release mode; Procfile runs `node index.js`. This infrastructure is third-party template material, not evidence of game implementation.

## Setup and testing

There is no playable Python program to launch. If inspecting the terminal template locally, review package.json and its native node-pty requirements in an isolated environment first. `npm test` is explicitly a placeholder that exits with an error. No install, server or tests were run here and no public deployment was verified.

Before implementing a game, define controls, board representation, food generation, growth and collision behavior. Test those rules separately from the terminal wrapper. Do not expose a process-spawning service publicly without reviewing access, resource limits and environment handling. The controller can write a creds.json file from CREDS; this update did not retrieve or use credentials.

## Snapshots

No screenshot was added. There is no real game state to capture. Future captures should show an implemented game using dated files in `docs/assets/`, not a stock image or invented board.

## Credits and licensing

Course/template and dependency rights remain unchanged. The existing package manifest declares ISC; no new license is added or applied to third-party material.

---

## Original README

![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

Welcome USER_NAME,

This is the Code Institute student template for deploying your third portfolio project, the Python command-line project. The last update to this file was: **August 17, 2021**

## Reminders

* Your code must be placed in the `run.py` file
* Your dependencies must be placed in the `requirements.txt` file
* Do not edit any of the other files or your code may not deploy properly

## Creating the Heroku app

When you create the app, you will need to add two buildpacks from the _Settings_ tab. The ordering is as follows:

1. `heroku/python`
2. `heroku/nodejs`

You must then create a _Config Var_ called `PORT`. Set this to `8000`

If you have credentials, such as in the Love Sandwiches project, you must create another _Config Var_ called `CREDS` and paste the JSON into the value field.

Connect your GitHub repository and deploy as normal.

## Constraints

The deployment terminal is set to 80 columns by 24 rows. That means that each line of text needs to be 80 characters or less otherwise it will be wrapped onto a second line.

-----
Happy coding!
