# typescript-cheatsheat


## types
Example 
```javascript
interface User {
  id?: number;
  firstname: string;
  lastname?: string;
  age: number;
  telephone?: number;
  twitter?: string;
}
```

#### Pick
```javascript
type UserFullname = Pick<User, 'firstname' | 'lastname'>;
```
#### Omit
```javascript
type UserPost = Omit<User, 'id'>;

const updateUser: UserPost = {
  firstname: 'Chris',
  lastname: 'Bongers',
  age: 32,
};

type UserPost = Omit<User, 'id'>;
```
