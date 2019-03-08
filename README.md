# pore
Binder repository for Nanopore data

To use this repository you will either need:

- Docker
- jupyter-repo2docker

or:

- conda

## Using repo2docker

```sh
git clone http://github.com/sdwfrost/pore
cd pore
jupyter-repo2docker -v .:$HOME .
```

## Using conda

```sh
git clone http://github.com/sdwfrost/pore
cd pore
conda env create -f binder/environment.yml
```

Running:

```sh
source activate pore
jupyter notebook --no-browser --ip='0.0.0.0'
```

Then open the link in your browser.

## Windows

See the following links to get repo2docker working on the Windows subsystem for Linux:

- [https://nickjanetakis.com/blog/using-wsl-and-mobaxterm-to-create-a-linux-dev-environment-on-windows](https://nickjanetakis.com/blog/using-wsl-and-mobaxterm-to-create-a-linux-dev-environment-on-windows)
- [https://nickjanetakis.com/blog/setting-up-docker-for-windows-and-wsl-to-work-flawlessly](https://nickjanetakis.com/blog/setting-up-docker-for-windows-and-wsl-to-work-flawlessly)