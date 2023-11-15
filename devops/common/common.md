# Common DevOps notes

## Detect and count languages in repository using Github Linguist

1. Build linguist

    ```bash
    git clone https://github.com/github-linguist/linguist.git
    cd linguist
    docker build -t linguist .
    ```

2. Get stats

    ```bash
    cd myrepo
    docker run --rm -v $(pwd):$(pwd) -w $(pwd) -t linguist github-linguist
    ```