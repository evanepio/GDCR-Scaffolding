
## Requirements

* These instructions work for Mac OS X. Tweak as appropriate
* Install Docker from [here](https://www.docker.com/) 
* Open 'Docker Quick Start Terminal'
* Search online repository: `docker search gcc`
* Pull the Mono image: `docker pull gcc` 
* Confirm the new image: `docker images`
* set `MY_SRC_HOME` to be appropriate directory on your computer
* execute the following (one command at a time):

<pre>
cd $MY_SRC_HOME
docker run --rm -it -v $(pwd):/data gcc
cd /data
chmod 744 ./run_tests.sh
</pre>

## To run tests

* `./run_tests.sh`
