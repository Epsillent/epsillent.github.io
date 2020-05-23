---
layout: page
title: Getting started with EpsEngine
permalink: /getting-started/
---

# Tutorial

1. Download our engine from [here](https://github.com/IvanHephaestus/EpsEngine)

2. create a **main.cpp** file and insert there following code

**main.cpp**
```c++
#include "Engine/Core.hpp"

int main(){
    Game *game = new Game();
    game->init();
    game->setupEveryting();
    for( ; ; ){
        game->networkFetch();
        game->doImportantCrap();
        game->renderEverything();
        game->swapBuffers();
    }
}

```

3. Well done, now you have created a Minecreaft
