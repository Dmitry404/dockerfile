# Ubuntu image with openJDK from ubuntu's packages - headless
FROM dmitry404/ubuntu-base
LABEL maintainer dmity404@gmail.com

RUN apt-get update && apt-get install -y --no-install-recommends \
        openjdk-8-jre-headless \
      && rm -rf /var/lib/apt/lists/*

CMD ["java", "-version"]
