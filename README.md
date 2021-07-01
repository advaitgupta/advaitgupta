<!-- Zero width character is used to put extra blank lines before and after code -->

<h3>
    
```c++
​
from __future__ import annotations

import json
from dataclasses import asdict, dataclass


@dataclass
class Arsenal:
    languages: tuple[str, ...] = ("C++", "JAVA")
    love: tuple[str, ...] = ("Coding", "Designing Algorithms")
    projects     : tuple[str, ...] = ("Battleship")
    upcoming  : tuple[str, ...] = ("RGPTI Banking System")

    def jsonify(self) -> str:
        return json.dumps(asdict(self), indent=4)


arsenal = Arsenal()
print(arsenal.jsonify())
​
```
</h3>
