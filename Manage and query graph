// 1. Create Nodes
CREATE (a:Person {name: 'Alice', age: 25});
CREATE (b:Person {name: 'Bob', age: 27});
CREATE (c:Person {name: 'Charlie', age: 30});
// 2. Create Relationships
CREATE (a)-[:FRIENDS_WITH]->(b);
CREATE (b)-[:FRIENDS_WITH]->(c);
CREATE (a)-[:COLLEAGUE_OF]->(c);
// 3. Retrieve All Nodes
MATCH (n) RETURN n;
// 4. Retrieve All Relationships
MATCH (a)-[r]->(b) RETURN a, r, b;
// 5. Display Specific Relationship
MATCH (a:Person)-[:FRIENDS_WITH]->(b:Person)
RETURN a.name AS Person1, b.name AS Person2;
