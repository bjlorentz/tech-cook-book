# Cookbook Maven

## Presentation

Some usefull command and plugins

## Cookbook Zone

### Execute one specific test in maven 

```
mvn test -Dtest=${TEST_CLASS_TO_EXECUTE}[#${METHOD_NAME}]
```

### Search dependency in dependency tree

```
mvn dependency:tree -Dincludes=[$GROUP_ID]:$ARTIFACT_ID [-Dverbose]

# Example - Import of commons-io
mvn dependency:tree -Dincludes=*:commons-io -Dverbose
```

## Plugin Zone

* Maven dependency-check : Analyze dependencies imported by the project and check if there are CVE associated with them. 
* Maven dependency : Allow to show dependencies tree of project. 
