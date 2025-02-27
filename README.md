Website using the static site generator [Jekyll](https://github.com/jekyll/jekyll).


The official docker image can be used to build the site and host it locally at http://localhost:4000:
```
docker pull jekyll/jekyll
docker run --rm \
  --volume="/path/to/fmonteghetti.github.io:/srv/jekyll:Z" \
  --publish [::1]:4000:4000 \
  jekyll/jekyll \
  jekyll serve
```
