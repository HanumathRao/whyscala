Scala
=====

* Student Questions about Scala
 * http://www.javacodegeeks.com/2012/02/student-questions-about-scala-part-1.html
 * http://www.javacodegeeks.com/2012/03/student-questions-about-scala-part-2.html
* Scala School by Twitter https://twitter.github.io/scala_school/ and Effective Scala http://twitter.github.io/effectivescala/
* The Neophyte's Guide to Scala
 * http://danielwestheide.com/scala/neophytes.html
 * http://danielwestheide.com/blog/archives/
* Resources for Getting Started With Functional Programming and Scala 
 * http://nerd.kelseyinnis.com/blog/2013/01/07/resources-for-getting-started-with-functional-programming-and-scala/
* Language
 * Scala's Types of Types http://ktoso.github.io/scala-types-of-types/ (Konrad ktoso Malawski)
* Cake Pattern
 * Component configuration http://fr.slideshare.net/DerekWyatt1/baking-delicious-modularity-in-scala (Derek Wyatt)
* Compiler
 * Useful Scalac Flags https://gist.github.com/tpolecat/8812750
 * wartremover https://github.com/puffnfresh/wartremover
* Scala Days 2014 http://www.parleys.com/channel/53a7d269e4b0543940d9e535/presentations?sort=views&state=public

Typeclasses
-----------
* JsonConverter, JsonWriter, Expression, ExpressionEvaluator. http://www.youtube.com/watch?v=sVMES4RZF-8 (Marakana)
* SO: Benefits http://stackoverflow.com/questions/13963070/scala-typeclass-example-how-to-explain-the-benefits
* Neophyte's Guide http://danielwestheide.com/blog/2013/02/06/the-neophytes-guide-to-scala-part-12-type-classes.html
* Raster Image Processing http://www.youtube.com/watch?v=D3VBVGhZ1SE
  * stephenjudkins / pureimage https://github.com/stephenjudkins/pureimage
* Typeclass Pattern - An Alternative to Inheritance http://www.youtube.com/watch?v=yYo0gANYViE

Presentations
-------------
* http://www.infoq.com/presentations/scala-tips-tricks
  * Type Aliases
  * Class Tag, Type Tag
  * Auto-lifted partial functions
  * NoStackTrace trait
  
  * Type Classes, Context Bounds, Implicitly
  * @ImplicitNotFound
  * Low Priority Default Implicits (Predef.scala)
  * ScalaDoc: where does SCala look for implicits?
  * Slides Implicits in Scala by Derek Wyatt
  * Neophyte's Guite to Scala by Daniel Westhside

News and Link hubs
------------------
* Scala Times http://us2.campaign-archive2.com/home/?u=ba834c562d82d9aba5eaf90ba&id=32cef9ab4e
* Awesome Scala https://github.com/lauris/awesome-scala

Distributed Systems, Akka
=========================
* Designing a Concurrent Application http://learnyousomeerlang.com/content (Learn you some Erlang)
* [Distributed Computing: Principles, Algorithms, and Systems](http://tnij.org/distributedcomputing) http://www.cs.uic.edu/~ajayk/DCS-Book
* Distributed systems meta list https://gist.github.com/macintux/6227368
* Distributed systems for fun and profit http://book.mixu.net/distsys/
* [Lesson learned] The network is reliable http://aphyr.com/posts/288-the-network-is-reliable
* Akka Clustering, Step by Step http://tersesystems.com/2014/06/25/akka-clustering/
* Distributed in Space and Time (Roland Kuhn @ Scalapeño 2014) https://parleys.com/play/545b4d2ae4b08fbc478d8bf9
* How Complex Systems Fail http://web.mit.edu/2.75/resources/random/How%20Complex%20Systems%20Fail.pdf
* A comprehensive study of Convergent and Commutative
Replicated Data Types http://hal.upmc.fr/inria-00555588/document

Akka
-----
* Scaling out with Akka Actors http://www.infoq.com/presentations/akka-scala-actors-distributed-system (Joshua Suereth)
 * Joshua Suereth designs a scalable distributed search service with Akka and Scala using actors, and covering practical aspects of how to scale out with Akka’s clustering API.
 * https://github.com/jsuereth/intro-to-actors
* [Concurrency Anti-patterns in Scala](http://www.youtube.com/watch?v=dCEZDlH1ygo)
* Scala IO Excercises https://github.com/RayRoestenburg/scala-io-exercise-1
* Cheat Sheets for Reactive Programming https://github.com/sjuvekar/reactive-programming-scala/blob/master/ReactiveCheatSheet.md
* The Road to Akka Cluster and Beyond (Jonas Bonér) http://www.slideshare.net/jboner/the-road-to-akka-cluster-and-beyond
* http://www.infoq.com/presentations/akka-design-patterns/ (Jamie Allen)
  * Guaranteed Delivery Doesn't Exist - Akka will do something at most once.
  * Mailboxes - Durable Mailboxes = don't; No guarantee the message will even get to the mailbox
  * We don't know what messages don't get to us
  * Build sources of truth, then make system respond to it. Things may get lost somewhere in between; Build Sentinels responsible for querying the source of truth and align actor to it
    * System is resilient to messages it didn't receive
    * System is less comples than attempting to guarantee no message loss
* A handful Akka techniques http://manuel.bernhardt.io/2014/04/23/a-handful-akka-techniques/

Akka at Conspire
----------------
* Akka at Conspire [Part 1]: How We Built Our Backend on Akka and Scala http://blog.goconspire.com/post/64130417462/akka-at-conspire-part-1-how-we-built-our-backend-on
* Akka at Conspire [Part 2]: Why We Like Actors http://blog.goconspire.com/post/64274254800/akka-at-conspire-part-2-why-we-like-actors
* Akka at Conspire [Part 3]: Making Your Akka Life Easier http://blog.goconspire.com/post/64412850756/akka-at-conspire-part-3-making-your-akka-life-easier
* Akka at Conspire [Part 4]: Don’t Fall Into Our Anti-Pattern Traps http://blog.goconspire.com/post/64780988287/akka-at-conspire-part-4-dont-fall-into-our
* Akka at Conspire [Part 5]: The Importance of Pulling http://blog.goconspire.com/post/64901258135/akka-at-conspire-part-5-the-importance-of-pulling

Papers
-------
* Probabilistically Bounded Staleness for Practical Partial Quorums http://www.eecs.berkeley.edu/Pubs/TechRpts/2012/EECS-2012-4.pdf (Peter Bailis)
 * Interactive demo http://pbs.cs.berkeley.edu/
* Readings in distributed systems http://christophermeiklejohn.com/distributed/systems/2013/07/12/readings-in-distributed-systems.html
* Dynamo: Amazon’s Highly Available Key-value Store http://www.read.seas.harvard.edu/~kohler/class/cs239-w08/decandia07dynamo.pdf
* Google MillWheel: Fault-Tolerant Stream Processing at
Internet Scale http://static.googleusercontent.com/media/research.google.com/pl//pubs/archive/41378.pdf

Congestion avoidance, backpressure
----------------------------------
* Congestion Avoidance and Control http://ee.lbl.gov/papers/congavoid.pdf (Van Jacobson)

JVM
===
* Garbage Collector
 * Everything I Ever Learned about JVM Performance Tuning @twitter http://www.infoq.com/presentations/JVM-Performance-Tuning-twitter
 * http://www.cubrid.org/blog/dev-platform/understanding-java-garbage-collection/
 * GC Tuning http://www.oracle.com/technetwork/java/javase/gc-tuning-6-140523.html
 * http://www.cubrid.org/blog/tags/Garbage%20Collection/
* ??
 * Choosing Executor Service http://blog.jessitron.com/2014/01/choosing-executorservice.html
* Enabling Java in Latency Sensitive Environments http://www.infoq.com/presentations/java-tuning-latency
 * Zing http://www.azulsystems.com/products/zing/whatisit
 * jHiccup https://github.com/giltene/jHiccup
 * TTSP - Time To Safe Point
 * Extreme outlier cost: Biased Locking, Counted loops optimization
 * Lock deflection, Weak references, Soft references, finalizers
 * THP - Transparent Huge Pages
 * Gil Tene @ InfoQ http://www.infoq.com/author/Gil-Tene
 * Choosing a Garbage Collector http://www.azulsystems.com/sites/default/files/images/Understanding_Java_Garbage_Collection_v3.pdf

Reactive Extensions
===================
* Src https://github.com/Netflix/RxJava/tree/master/language-adaptors/rxjava-scala
* Examples https://github.com/samuelgruetter/rx-playground
* End-to-End Reactive Netflix (javascript) http://www.infoq.com/presentations/reactive-programming-netflix
* Asynchronous Programming at Netflix http://www.infoq.com/presentations/async-programming-netflix
  * map, filter, switchLatest, throttle, concatAll, retry

Big Data
========
* Big Data using Scala https://speakerdeck.com/samklr/big-data-using-scala
 * Scalding, Spark
* Databricks makes Hadoop and Apache Spark easy to use http://www.zdnet.com/databricks-makes-hadoop-and-apache-spark-easy-to-use-7000031115/
  * The company is offering a cloud service, Databricks Cloud, that makes it possible for organizations to quickly get started with Apache Spark. Databricks Cloud handles the metadata, launching and provisioning a Spark Cluster, and makes it easy for that cluster to process an organization's data stored in Amazon's S3 service.
  * Databricks cloud helps analysts by organizing the data into "notebooks" and making it easy to visualize data through the use of dashboards. It also makes it easy to analyze data using machine learning (MLib), GraphX and Spark SQL.
* Spark should be better than MapReduce (if only it worked) http://blog.explainmydata.com/2014/05/spark-should-be-better-than-mapreduce.html?m=1 (Alex Rubinsteyn)
* Hands-on Exercises http://ampcamp.berkeley.edu/big-data-mini-course/
* Summingbird: A Framework for Integrating Batch and
Online MapReduce Computations http://www.vldb.org/pvldb/vol7/p1441-boykin.pdf

Functional Programming
======================
* Functional Talks http://functionaltalks.org/
* Functional programs rarely rot http://michaelochurch.wordpress.com/2012/12/06/functional-programs-rarely-rot/
 * The problem, rather, is that stateful programs evolve in bad ways when programs get large.
 * Such functions actually have precise (and usually, obviously intended) semantics which means that it’s clear what is and what is not a bug, and unit testing is relatively straightforward.
 * An unbounded amount of intermediate stuff can be shoved into an imperative program, with no change to its interface. Or, to put it another way, with a referentially transparent function, the interface-level activity is all one needs to know about its behavior.
 * Mutable state is an important tool, but it should almost always be construed as a performance-oriented optimization.
 * No, there’s nothing innately superior about functional programming, but the style forces people to deal with the complexity they generate by forcing it to live at the interface level. You can’t, as easily, throw a dead rat in the code to satisfy some dipshit requirement and then forget about it.

Play Framework
==============
* Play Framework at LinkedIn http://www.slideshare.net/brikis98/the-play-framework-at-linkedin
* Play Framework: async I/O http://www.slideshare.net/brikis98/play-framework-async-io-with-java-and-scala
* Ultimate Guide to get started http://brikis98.blogspot.ca/2014/03/the-ultimate-guide-to-getting-started.html
    * Composable and Streamable Play apps http://www.ustream.tv/recorded/44303071
        * https://github.com/brikis98/ping-play
        * http://www.slideshare.net/brikis98/composable-and-streamable-play-apps
 
* Optimizing Play for Production https://www.youtube.com/watch?v=cnPPLpIk9mo (James Ward)

IntelliJ IDEA
=============
* Working With IntelliJ IDEA (+VisualVM) http://www.scalacourses.com/student/showLecture/80
* Tips & Tricks (30 Days...) http://blog.jetbrains.com/idea/category/tips-tricks/

Scala.js
========
* http://www.scala-js.org/ and https://github.com/scala-js/scala-js
* http://www.scala-js-fiddle.com/
* Live coding http://vimeo.com/87845442 by Li Haoyi 

Jobs
====
* Typesafe Together http://typesafe.com/how/together/our-customers-are-hiring
