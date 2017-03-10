# neo4jlearning
//https://community.risingstack.com/graphs-graphdbs-and-javascript-exploring-trumpworld/
$ docker pull neo4j:3.1.0
$ docker run -d -p 7474:7474 -p 7687:7687 -v ~/data:/data --name neo4j neo4j:3.1.0

## Symple Syntax
```
MATCH (p:Person {name: "Alex"})  
RETURN p; 
```

```
MATCH (p:Person)  
RETURN p;  
```

```
(p1:Person {name: "Alex"})-[r:Knows]-(p2:Person {name: "Susan"})  
RETURN p1, r, p2;  
```

```
MATCH (p1:Person {name: "Alex"})-[r:Knows]-(p2:Person)  
RETURN p1, r, p2;  
```

```
MATCH (p1:Person)-[]-(p2:Person)  
RETURN p1, p2;  
```

```
MATCH (p1:Person {name: "Susan"})-[r:Knows*2]-(p2:Person {interest: "business"})  
RETURN p1, r, p2;  
```

## Bolt
https://neo4j.com/blog/neo4j-3-0-language-drivers/

## Neo4j API Javascript-driver Docummentation
http://neo4j.com/docs/api/javascript-driver/current/

## Neo4j Sandbox
https://neo4j.com/sandbox-v2/

