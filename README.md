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

const userName: UserFullname = {
  firstname: 'Chris',
  lastname: 'Bongers',
};
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

#### Partial
```javascript
type UserFullname = Partial<User>; // it means all fields optionals

const userName: UserFullname = {
  firstname: 'Chris',
  age: 22,
};
```
