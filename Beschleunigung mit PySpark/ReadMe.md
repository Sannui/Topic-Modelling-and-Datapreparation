## Beschleunigung mithilfe von PySpark
PySpark wurde von den Entwicklern des Big-Data-Systems Apache Spark herausgebracht und ist eine Version, welche in der Python Programmierung Anwendung findet. Die Architektur verteilt sich auf ein Cluster, wodurch es ermöglicht wird große Datenmengen zu parallelisieren und performanter zu verarbeiten. Hierfür wird auf den Arbeitsspeicher der Hardware zugegriffen wodurch die Festplatte nicht belastet wird (Wuttke, Einführung in Apache Spark: Komponenten, Vorteile und Anwendungsbereiche, 2022). Es gilt als eines der besten Frameworks in der Datenwissenschaft und verbindet Big Data mit maschinellem Lernen, da es sowohl In-Memory-Operationen für eine bis zu 100-fache Beschleunigung liefert als auch Zusatzpakete wie MLib und GraphX bietet. Spark läuft auf einer Virtuellen Maschine von Java (JVM), ist in Scala geschrieben und auf Hadoop/HDFS implementiert. PySpark ist die Python-API, welche eine Schnittstelle zwischen der Python-Programmierung und dem Spark-Framework liefert. Auf diese Weise ist es möglich mithilfe von Objekten die Vorteile von Spark zu nutzen, ohne die Programmiersprache Scala zu erlernen (Sarkar, 2018).
Um mit Apache Spark in Juyter Notebooks arbeiten zu können, muss die richtige Version zuerst heruntergeladen werden. Hierfür kann auf der Webside von Apache Spark die richtige Version heruntergeladen werden. In Abbildung sechs sind die notwendigen Konfigurationen ersichtlich (Apache Spark, 2023).

<center><img src="Apache_Download.png" height="300px" width="1100px"/></center>

<center>Herunterladen von Spark 3.3.1 (Apache Spark, 2023)</center>

Nun kann die Library über den „pip install“ Befehl oder über das Terminal installiert werden. In diesem Fall hat die Installation über das Terminal stattgefunden. Nach der erfolgreichen Installation von pyspark können die für die Beschleunigung des Ladevorgang benötigten Klassen importiert werden. Wichtig ist jedoch, dass zuvor „findspark“ importiert und initialisiert wurde, damit die benötigte Spark Instanz gewunden wird (Shah, 2018).

```
# Import findspark
import findspark
findspark.init()
```

Nach dem Erfolgreichen Abschluss aller Installationen und Imports, kann als nächstes eine Spark Session mit folgendem Befehl gestartet werden (Shah, 2018):