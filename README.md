# Sbt base image

This image is configured with a workdir `/app`, so to build your project you have to mount your project in '/app' (or change the working dir).
To see an example, have a look at the the docker-compose.yml. Keep in mind this image is intended for developping and building applications, not to deploy them.

To speed up your builds, you can mount your ~/.ivy2 cache at /root/.ivy2 in order to keep your artefacts even if your recreate a container from the image.
