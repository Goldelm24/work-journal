Nextjs Is a framework for building fast and search engine friendly applications. Today I learned about Data fetching and caching.


```
  const UsersPage = async () => {
  const res = await fetch('https://jsonplaceholder.typicode.com/users', { cache: 'no-store'});
  const users: User[] = await res.json(); 
```