# Release tool for elasticsearch plugin

This tool set allows release of elasticsearch plugins.

Copy `dev-tools/release.py` script to your `dev-tools/` dir and launch it using:

```sh
python3 dev-tools/release.py
```

or run in your root repository:

```sh
wget https://raw.githubusercontent.com/elasticsearch/elasticsearch-plugins-script/master/dev-tools/release.py -x -nH --cut-dirs=3
python3 dev-tools/release.py
```

It will download all needed scripts and files in a `plugin_tools` directory and will launch
the release process.

Note:

* We only download a new version if no one is available or if you did not launch the
release process for a long time
* If you need to force an update, you just have to remove `plugin_tools` dir
* You should add `plugin_tools` to your `.gitignore` file
* The `release.py` auto updates if needed. It means you will have to commit it to your repo.

