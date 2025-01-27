# ObjectiveNet

ObjectiveNet is an open source software to help people build causal networks of objectives, actions, and potentialities.

## Usage

To start ObjectiveNet:

- [install Docker](https://www.docker.com/get-started/) if not already on your machine,
- clone the repo (e.g. by running ```git clone https://github.com/planningcommons/objectivenet.git``` from a terminal),
- run ```docker compose up``` from the cloned *objectivenet/* directory,
- wait for it to start...and that's it! you can access it at [http://localhost:5173/](http://localhost:5173/) from a browser.


### Backend API

ObjectiveNet's graph database can also be queried directly using its backend API framework.
You can find its API schema at: http://localhost:8000/docs (generated automatically using Swagger).


## Development

This project uses:
- [FastAPI](https://fastapi.tiangolo.com/) framework and a [JanusGraph](https://janusgraph.org/) graph database on the backend,
- [Vue.js](https://vuejs.org/), [Vite](https://vite.dev/), and [Vue Flow](https://vueflow.dev/) on the frontend.


### Contributing

Looking to file a bug report or a feature request? https://github.com/planningcommons/objectivenet/issues

You can also contribute to ObjectiveNet by:
- experimenting with the software and directly [sending feedback via email](mario.morvan@ucl.ac.uk),
- creating feature/ or fix/ branches and opening [pull requests](https://github.com/planningcommons/objectivenet/pulls).


### Dev tools

Run `pre-commit install` to set up the git hook scripts. It'll perform some formatting, linting and unit tests before any commit.

To generate new *.txt* requirements files from *.in*, you'll need pip-tools: ```pip install pip-tools```<br>
Then, you can run: ```pip-compile requirements.in``` or ```pip-compile requirements-dev.in``` whenever you update these `.in` files.


## License

This project is licensed under the GNU Affero General Public License - see the [COPYING](COPYING) file for details.

© 2024 Mario Morvan
