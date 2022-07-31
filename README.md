[![Build Status](https://travis-ci.org/enelson/java_monads.svg?branch=master)](https://travis-ci.org/enelson/java_monads)
![tag](http://img.shields.io/github/tag/enelson/java_monads.svg)
[![Coverage Status](https://codecov.io/github/enelson/java_monads/coverage.png?branch=master)](https://codecov.io/github/enelson/java_monads?branch=master)
[![Javadoc](https://javadoc-emblem.rhcloud.com/doc/com.github.enelson/monads/badge.svg)](http://www.javadoc.io/doc/com.github.enelson/monads)

# Common Monads for Java

[![Monad](http://adit.io/imgs/functors/bind_def.png)](http://adit.io/posts/2013-06-10-three-useful-monads.html)

There is a great article [here](http://adit.io/posts/2013-06-10-three-useful-monads.html) that talks about 3 very common and useful monads: `Reader`, `Writer` and `State`. 

## Reader

The `Reader` monad allows a common context (ie. DAO object) to be threaded through to chained functions. A common use for this type of monad is dependency injection.

http://eed3si9n.com/learning-scalaz/Reader.html  
http://blog.originate.com/blog/2013/10/21/reader-monad-for-dependency-injection/

## Writer

The `Writer` monad is used to keep a running log of chained computations. For instance, if you have multiple arithmetic functions chained together, the writer class can append to the log each time a computation is run, and the final result will contain both the final value of the computations, as well as the complete log.

http://eed3si9n.com/learning-scalaz/Writer.html  
http://www.lispplusplus.com/2011/10/scala-writer-monad.html  
http://blog.tmorris.net/posts/the-writer-monad-using-scala-example/

## State

The `State` monad can be seen as similar to the reader monad, except that the state can be modified throughout the call chain, whereas the reader's context can only be read. 

http://eed3si9n.com/learning-scalaz/State.html  
https://softwarecorner.wordpress.com/2013/08/29/scalaz-state-monad/

Test
