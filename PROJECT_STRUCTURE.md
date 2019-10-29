# Folder structure

```
app-_some_center/
    components/ // => stateless components 
      Button/
        Button.tsx
        Button.spec.tsx
        Buttons.scss
        index.ts
    containers/ // => stateful components
      User/
        List/
          List.tsx
          List.spec.tsx
          List.scss
          utils.ts // => if needed
          index.ts
        Edit/
          ...
        Detail/
          ...
        index.ts  
    utils/ // => utils
      string/
        string.util.ts
        string.util.spec.ts
    models/ // => only for data models
      User/
        User.model.ts
        schema.ts
        validation.ts
    services/
      api/ // => for work with API
        User/
          User.service.ts
          User.service.spec.ts
          index.ts
      session/ => for other services
        session.service.ts
        session.service.spec.ts
    auth/
      Auth.service.ts
    assets/ // => additional assets
    styles/ // => styles folder
    context/ // => application's contexts
    
```

# Naming convention

### Interfaces

Interface's name should contain only base name of entity

### Classes

Class's name should be created from interface's name and **Model** word

Example: 
```
interface User {}
class UserModel implements User {}
```

### Boolean variables

Boolean variable should start from **is** or **has** prefix
Example:
```
const isUserActive: boolean;
const hasUserAccess: boolean;
```