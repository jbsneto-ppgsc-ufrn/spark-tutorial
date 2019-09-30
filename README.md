# Spark Tutorial

Apache Spark tutorial using Zeppelin notebooks.

**Requirement**: [Docker][0] installed and running.

Open the Terminal and enter the tutotial folder:

`$ cd /path/to/spark-tutorial`

Then, execute the following command:

`
$ docker run -p 8080:8080 --rm -v $PWD/data:/data -v $PWD/notebook:/notebook -e ZEPPELIN_NOTEBOOK_DIR='/notebook' --name zeppelin apache/zeppelin:0.8.1
`

This command will download the Zeppelin dependencies (approximately 3GB) and run it.

To see if Zeppelin is running and the notebooks available, visit the URL [localhost:8080/][1]

Test if Zeppelin is working by opening the notebook with the *Word Count* example:

* [Word Count - Scala][2]
* [Word Count - Python][3]

To execute the codes in the notebooks, click the play button or select the paragraph and use the shortcut `Shift + Enter`

Other notebooks available:

* [Outlier Detection: An ETL Tutorial with Spark - Scala][4]
* [Outlier Detection: An ETL Tutorial with Spark - Python][5]

[0]: https://www.docker.com/
[1]: http://localhost:8080/
[2]: http://localhost:8080/#/notebook/2ERGJNXED
[3]: http://localhost:8080/#/notebook/2ER9EUWBB
[4]: http://localhost:8080/#/notebook/2EQQ6BAV6
[5]: http://localhost:8080/#/notebook/2ERRY1XRJ