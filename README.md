# Puravid PlantUML sprites

This repository contains PlantUML sprites which can easily be used in PlantUML diagrams for nice visual representation of popular technologies.

This project is inspired in other PlantUML sprites repositories like [AWS-PlantUML](https://github.com/milo-minderbinder/AWS-PlantUML) and [PlantUML Icon-Font Sprites](https://github.com/tupadr3/plantuml-icon-font-sprites).
and [Cloudinsight PlantUML sprites](https://github.com/rabelenda/cicon-plantuml-sprites)

## Usage

Just import the proper sprite into your PlantUML diagram and use it like any other sprite.

Example:

```
@startuml
!define SPRITESURL https://raw.githubusercontent.com/rabelenda/cicon-plantuml-sprites/v1.0/sprites
!define PVIDAURL https://raw.githubusercontent.com/jagedn/mn-plantuml-sprites/master/sprites/

!includeurl SPRITESURL/java.puml
!includeurl SPRITESURL/cassandra.puml
!includeurl SPRITESURL/nodejs.puml
!includeurl SPRITESURL/kafka.puml
!includeurl SPRITESURL/tomcat.puml
!includeurl SPRITESURL/server.puml
!includeurl SPRITESURL/python.puml

!includeurl PVIDAURL/micronaut.puml

title Hello

skinparam monochrome true

actor User
rectangle "<$nodejs>\nwebapp" as webapp

rectangle "<$micronaut>\nAPI" as api
interface "<$kafka>\nEvents" as kafka
file "<$server>\nStorage" as repo
rectangle "<$java>\ncatalog" as catalog
rectangle "<$python>\nusers" as users

User -> webapp
webapp --> api
api -> repo
repo -> api
api ..> kafka
api --> catalog
api --> users
@enduml
```

![Example](https://www.plantuml.com/plantuml/png/ZP7FQXin4CRlUWebzEhTzbgAIQ216demSTDJBsFjUArO6edHoA5lNrdo1Y-qIm_Bpf-VlaypUaW2BDaxTJVWmHBgtVPvy-Dfz_ByNHz5OlhSzmnltMZbcFSv8Pj0WYIT2RvqzkYG1kYDBVLLT40NjLMAR0LJV_xKVUoloRl5zkVcw-F_6Rp2Y0Fr_Y_I7f8WzrEgr9qbu_A0cTtD54NY35qi9_y564W9QE1bYiA0hsaHES7Xj2mYmHkGHIGXdv4NaVXRZe4QCcEcnVRU6Wu4MQwGM76elw5pGQbqiXI1mMiVA9WZ1uzQEADIO2ImVad8Yj48q5YEtN_vq8PV_w8tt4ECzngIRg6QW-_6XNtSRYe8qIfBWdm0Kw6wfm8ydP4aLQQMrC4sbRQ3GkmaC8nO4SOOvcQNbosG0G4NnWfTupdNzbN8N8IRNusKkaogL-jfblRJgrAvNBfyfJaPnw1lwbstRfTkLEbCrbFUB1wGXkpT7m00)


## Note

* All logo icons are the registered trademarks of their respective owners.
