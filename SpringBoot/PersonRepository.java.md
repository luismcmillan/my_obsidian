[[Projektstruktur]]
```Java
package com.example.springbootexample.repository;

import com.example.springbootexample.model.Person;
import org.springframework.data.jpa.repository.JpaRepository;

public interface PersonRepository extends JpaRepository<Person, Long> {
}

```