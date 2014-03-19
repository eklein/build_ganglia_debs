Docker ganglia debs
===================

This is a simple Dockerfile to build up an image and create debs for whichever version you want.

3.7.0 is in the Dockerfile right now because that's what I was building.  Update it to whichever version you prefer.

You would use it to build debs (I was building debs from master) as such:

```
docker build -rm -t ganglia_master_debs .
```

Once it's complete, you can launch the image to copy the debs off by running:

```
docker run -i -t ganglia_master_debs /bin/bash
```
