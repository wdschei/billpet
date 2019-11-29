Clone this repo.

* **NOTE:** If the phrase _clone the repo_ is new to you, then check out this [tutorial](https://guides.github.com/activities/hello-world/).

The contents of this repo are based on this [turorial](http://jmcglone.com/guides/github-pages/).

To isolate the [Jekyll](https://jekyllrb.com/docs/)/Ruby environment from the rest of your machine, you can use Docker.
You can set up Docker in a Windows environment using this [tutorial](https://docs.docker.com/docker-for-windows/)

Once you are able to run the `Hello World` container using the command:

> `$ docker run hello-world`

Then you are ready to look at the site contained in the local clone of the repository by issuing the following command:

> `$ docker run --rm --volume="$PWD:/srv/jekyll" -p 4000:4000 -it jekyll/minimal:3.8.5 jekyll serve`

You can view the local site at:

* http://localhost:4000

OR on Windows, it is typically at:

* http://192.168.99.100:4000

Remember that when any changes are saved to the local cloned pages, Jekyll automagically detects this and rebuilds them in the `_site` directory which is what is being served locally.
This provides a very fast and local feedback loop to test changes before `commit`'ing and `push`'ing them to be published publicly.

The currently published site based on the `gh-pages` branch can be viewed at:

* http://BillPet.TheScheideggers.com
