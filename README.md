# typescript-cheatsheat


## types
#### Pick
```javascript
interface User {
  id?: number;
  firstname: string;
  lastname?: string;
  age: number;
  telephone?: number;
  twitter?: string;
}
type UserFullname = Pick<User, 'firstname' | 'lastname'>;
```

#### Omit
type UserPost = Omit<User, 'id'>;

const updateUser: UserPost = {
  firstname: 'Chris',
  lastname: 'Bongers',
  age: 32,
};

type UserPost = Omit<User, 'id'>;
