# pip

Dockerized pip

# Usage

To install some package (e.g. boto) onto the current directory (useful for packaging functions).

docker run --rm -v $(pwd):/src \
    --user $UID \
    binaris/pip \
    install boto -t .

(`/src` is the working directory of the image)
