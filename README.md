pathfinder_graph_reactome [![Phovea][phovea-image]][phovea-url] [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url]
=====================

Preparation
-----------

1. Download http://reactome.org/download/current/reactome.graphdb.tgz
1. Extract to directory
1. rename `reactome.graph.db` to `graph.db` and nest it within a `databases` directory
1. tar.gz it again to `db_neo4j_reactome.tar.gz` such that it contains `databases/graph.db/...`
1. move it `_backup`
1. run `./docker-backup restore` to restore the db snapshot
1. start Pathfinder as usual
1. open: http://localhost:8080/main.html?uc=reactome

Installation
------------

```
git clone https://github.com/Caleydo/pathfinder_graph_reactome.git
cd pathfinder_graph_reactome
npm install
```

Testing
-------

```
npm test
```

Building
--------

```
npm run build
```



***

<a href="https://caleydo.org"><img src="http://caleydo.org/assets/images/logos/caleydo.svg" align="left" width="200px" hspace="10" vspace="6"></a>
This repository is part of **[Phovea](http://phovea.caleydo.org/)**, a platform for developing web-based visualization applications. For tutorials, API docs, and more information about the build and deployment process, see the [documentation page](http://phovea.caleydo.org).


[phovea-image]: https://img.shields.io/badge/Phovea-Server%20Plugin-10ACDF.svg
[phovea-url]: https://phovea.caleydo.org
[npm-image]: https://badge.fury.io/js/pathfinder_graph_reactome.svg
[npm-url]: https://npmjs.org/package/pathfinder_graph_reactome
[travis-image]: https://travis-ci.org/Caleydo/pathfinder_graph_reactome.svg?branch=master
[travis-url]: https://travis-ci.org/Caleydo/pathfinder_graph_reactome
[daviddm-image]: https://david-dm.org/Caleydo/pathfinder_graph_reactome/status.svg
[daviddm-url]: https://david-dm.org/Caleydo/pathfinder_graph_reactome
