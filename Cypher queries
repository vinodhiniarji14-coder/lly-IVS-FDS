// 1. Find all people older than 26
MATCH (p:Person)
WHERE p.age > 26
RETURN p.name, p.age;
// 2. Count how many FRIENDS_WITH relationships exist
MATCH (:Person)-[r:FRIENDS_WITH]->(:Person)
RETURN COUNT(r) AS TotalFriendships;
// 3. Find friends of a particular person (Alice)
MATCH (a:Person {name: 'Alice'})-[:FRIENDS_WITH]->(friends)
RETURN friends.name AS FriendsOfAlice;
// 4. Find mutual connections
MATCH (a:Person)-[:FRIENDS_WITH]->(b:Person)-[:FRIENDS_WITH]-
>(c:Person)
RETURN a.name AS Person, c.name AS MutualConnection;
