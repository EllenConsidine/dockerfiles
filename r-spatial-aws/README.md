# r-spatial-aws

Docker container with R, RStudio, various spatial packages, and the tidyverse, based on the [rocker/geospatial](https://github.com/rocker-org/geospatial) image.

## How to use

To use Rstudio:

```
docker run -e PASSWORD=yourpassword -d -p 8787:8787 earthlab/r-spatial-aws
```

In a web browser, navigate to localhost:8787.
Log in with username: rstudio, and the password your provided in your call to `docker run`.

## Mounting folders

If you want to share a directory between your host machine and the container, use the `-v` flag in your call to `docker run`, as described [here](https://github.com/rocker-org/rocker/wiki/Sharing-files-with-host-machine).
For more information on how to take full advantage of RStudio in this image, see https://github.com/rocker-org/rocker/wiki/Using-the-RStudio-image.
