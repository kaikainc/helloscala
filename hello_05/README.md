包机制之一
=========
scala 的包，可以不对应目录结构

Utils.scala 增加
package com.mine.hello

scalac Utils.scala

HelloWorld.scala 增加
import com.mine.hello._

scalac -cp . HelloWorld.scala
scala -cp . Hello

java -cp .:/home/hde/scala-2.12.11/lib/scala-compiler.jar:/home/hde/scala-2.12.11/lib/scala-library.jar Hello