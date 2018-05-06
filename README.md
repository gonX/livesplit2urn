About
-----
This is a small BASH script to convert [LiveSplit](http://livesplit.github.io/) .lss files to [Urn](https://github.com/3snowp7im/urn)-compatible JSON files.

Dependencies
============
- [jq](https://stedolan.github.io/jq/)
- [xml2json-command](https://www.npmjs.com/package/xml2json-command)

Usage
-----
```
./livesplit2urn livesplit-splits.lss > urn-splits.json
```

The script returns the direct output from `jq`.

Pitfalls
--------
- If you have multiple split times (e.g. additional imported splits), the script will likely not provide a proper output.
- Urn's `best_time` is currently unpopulated.

Also
----
Pull requests are welcome.
