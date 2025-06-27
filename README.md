# <a src="https://qalipsis.io"><img src="http://assets.qalipsis.io/qalipsis-logo.png" style="height:60px;width:60px;position:relative;top:18px;margin-right:20px;"/>QALIPSIS - Scenario developer platform</a>

## Introduction

This repository contains the scenario developer platform (aka Maven Bill of Materials or BOM) to develop scenario for QALIPSIS, an enterprise-grade load and performance-testing tool especially
designed for distributed systems. It is a step above other load test applications that merely evaluate your system
internally.

* QALIPSIS is developer-centric with a low learning curve that makes it easy to use and extremely efficient.
* QALIPSIS is developed in Kotlin to gain the benefits of the Java ecosystem and provide seamless system performance.
* QALIPSIS is designed to test the performance of distributed and monolithic systems.
* QALIPSIS collects data from operating systems, databases, and monitoring tools.
* QALIPSIS cross-checks system metrics and performs data verification to ensure that the test systems is performing as
  expected.

## How to use it?

In your build.gradle file, add the following dependency to your scenario:

```
dependencies {
    implementation(platform("io.qalipsis:qalipsis-platform:<version>"))
    kapt(platform("io.qalipsis:qalipsis-platform:<version>"))
    
    // Add your plugins:
    implementation("io.qalipsis.plugin:qalipsis-plugin-cassandra")
    implementation("io.qalipsis.plugin:qalipsis-plugin-jackson")
    
    // Add the additional libraries you need:
    implementation("io.kotest:kotest-assertions-core:5.4.2")
}
```

## Official website

You can learn more about QALIPSIS under https://qalipsis.io.

## Documentation

The complete documentation of QALIPSIS is available under https://docs.qalipsis.io.

## Examples

You can find examples of QALIPSIS scenarios under https://github.com/qalipsis/qalipsis-examples.

## License

The QALIPSIS scenario developer platform is distributed under the GNU Affero General Public License 3.0, the terms can
be
read [here](./LICENSE).