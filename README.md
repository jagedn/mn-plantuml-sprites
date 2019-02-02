# Puravid PlantUML sprites

This repository contains PlantUML sprites which can easily be used in PlantUML diagrams for nice visual representation of popular technologies.

This project is inspired in other PlantUML sprites repositories like [AWS-PlantUML](https://github.com/milo-minderbinder/AWS-PlantUML) and [PlantUML Icon-Font Sprites](https://github.com/tupadr3/plantuml-icon-font-sprites).
and [Cloudinsight PlantUML sprites](https://github.com/rabelenda/cicon-plantuml-sprites)

## Usage

Just import the proper sprite into your PlantUML diagram and use it like any other sprite.

Example:

```
@startuml
!define PURAVIDAURL https://gitlab.com/puravida-asciidoctor/plantuml-sprites/raw/master/sprites
!define SPRITESURL https://raw.githubusercontent.com/rabelenda/cicon-plantuml-sprites/v1.0/sprites

!includeurl SPRITESURL/tomcat.puml
!includeurl SPRITESURL/kafka.puml
!includeurl SPRITESURL/java.puml
!includeurl SPRITESURL/cassandra.puml
!includeurl PURAVIDAURL/micronaut16z.puml

title Micronaut example

skinparam monochrome true

rectangle "<$tomcat>\nwebapp" as webapp
queue "<$kafka>" as kafka
rectangle "<$java>\ndaemon" as daemon
database "<$cassandra>" as cassandra

webapp -> kafka
kafka -> daemon
daemon --> cassandra 

@enduml
```

![Example](https://www.planttext.com/plantuml/img/XL7BJiCm4BpxAzoAQv8xGb4bn0690shXXeGszZPnunVsclBvs4vKbGDmMNbsnpCxzYuI14f6CxQHU5GM-U5v__ZoS7X_tJ_nYSZ7swuBS6v7HLCQKiGWd2Mqr0fdycH0ZLP29rJkDrw3BNfDz44Hniv090pT2jb6MQ6Jn1JqjLD7pWYWrfTLVkFCS9pXRye9FlzX28WHh0mhZP4YZVnUkoILZMgSYA-xSlm2upKo5cTbFGGmt3Zhn1ISGKuXvL50GM37BB6zkrb2z6-Mdt40xxSS8b-Qx2DXggIQeg-ZUlmfKG8K0GcOlIghj9W4WW5YvLmYB2eNcCDKBzxqgtIj1LQDKdYJqTMDNVwx-WwCVGC0)


## Note

* All logo icons are the registered trademarks of their respective owners.
