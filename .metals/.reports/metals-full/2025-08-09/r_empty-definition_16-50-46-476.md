error id: file:///C:/Users/Admin/LFX-Mentorship/LFX-Mentorship/build.sbt:`<error>`#`<error>`.
file:///C:/Users/Admin/LFX-Mentorship/LFX-Mentorship/build.sbt
empty definition using pc, found symbol in pc: 
empty definition using semanticdb
empty definition using fallback
non-local guesses:
	 -scalaVersion.
	 -scalaVersion#
	 -scalaVersion().
	 -scala/Predef.scalaVersion.
	 -scala/Predef.scalaVersion#
	 -scala/Predef.scalaVersion().
offset: 53
uri: file:///C:/Users/Admin/LFX-Mentorship/LFX-Mentorship/build.sbt
text:
```scala
// See README.md for license details.

ThisBuild / @@scalaVersion     := "2.13.10"
ThisBuild / version          := "0.1.0"
ThisBuild / organization     := "com.github.merledu"

val chiselVersion = "3.5.5"

lazy val root = (project in file("."))
  .settings(
    name := "LFX-2025",
    libraryDependencies ++= Seq(
      "edu.berkeley.cs" %% "chisel3" % chiselVersion,
      "edu.berkeley.cs" %% "chiseltest" % "0.5.6" % "test",
      "org.scalatest" %% "scalatest" % "3.2.0" % "test",
    ),
    scalacOptions ++= Seq(
      "-language:reflectiveCalls",
      "-deprecation",
      "-feature",
      "-Xcheckinit",
      "-Ymacro-annotations",
    ),
    addCompilerPlugin("edu.berkeley.cs" % "chisel3-plugin" % chiselVersion cross CrossVersion.full),
  )

```


#### Short summary: 

empty definition using pc, found symbol in pc: 