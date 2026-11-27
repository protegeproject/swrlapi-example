# SWRLAPI example

A small Java application demonstrating SQWRL query execution through SWRLAPI.
The `protege-6` branch uses **2.1.5-SNAPSHOT / OWLAPI 5.5.1**. The
[complete source](src/main/java/org/swrlapi/example/SWRLAPIExample.java) runs
`swrlb:add(?x, 2, 2) -> sqwrl:select(?x)` and prints `x: 4`.

## Build and run

Use JDK 17 / Maven 3.9 and the `protege-6` sibling checkouts from the build guide.
From the workspace root:

```sh
mvn -B -f swrlapi-project/pom.xml -Pcore,nullness,static-analysis clean verify
java -jar swrlapi-example/target/swrlapi-example-2.1.5-SNAPSHOT-jar-with-dependencies.jar
```

An optional final argument supplies an ontology document, for example
`java -jar swrlapi-example/target/swrlapi-example-2.1.5-SNAPSHOT-jar-with-dependencies.jar ontology.owl`.
No Protégé installation or ontology file is required for the arithmetic example.
You can also import the sibling Maven projects into an IDE. This sample is a
Java application; OSGi contributors use the separate
[built-in registration example](https://github.com/protegeproject/swrltab-plugin/blob/protege-6/docs/built-in-registration.md).

[Build guide](https://github.com/protegeproject/swrlapi-project/blob/protege-6/README.md) · [Runbook](https://github.com/protegeproject/swrlapi-project/blob/protege-6/ops/runbook.md) · [Roadmap](https://github.com/protegeproject/swrlapi-project/blob/protege-6/ops/roadmap.md)

## License

[BSD 2-Clause](license.txt), copyright Stanford University.
