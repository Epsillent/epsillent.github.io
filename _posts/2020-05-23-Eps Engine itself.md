---
layout: post
title: EpsEngine itself
categories: [Miscellaneous]
---

well, here is a whole eps engine documentation post

*c++ code block*
```c++
static int __init init(const char *argc, ...){
    doShit();
}
```
##### Plan
* Application layer
    * Window System
    * Input System
    * Event System(with callbacks)
    * Callbacks( or something like signals and slots)
* Engine 
    * Perfomance measure
* Memory managment
    * TypeAlocator
    * StaticAllocator
    * StackAllocator
* Render system
    * Flexible API
        * Drawing primitives
        * SFML compat profile
    * Renderer
    * Camera2D

* Scene
    * Sprite2D
    * SceneGraph
* Physics
    * Basic Collision detection
    * Forces
    * Rigidbody
* OS
    * Data types
    * Sockets
    * Threading
    * File I\O
* Assets
    * Resource Manager
        * VFS
        * font cache
        * strings cache
        * texture cache
        * audio cache
* UI
    * Constraint layout
    * Base Widget
    * Widgets
    * Animations
* Scripting
    * Lua integration

    
***
### Desired code style

1. File names are all lowercase with underscores             
>file_name.cpp

2. Namespaces names are all lowercase                        
>namespace_name::

3. Class and structures names are mixed case                 
>SomeClass

4. functions are all lowercase with underscores             
>yet_another_fucntion();

5. Class members are lowercase and have m_ prefix              
>m_class_member

6. const variables have k_ prefix                           
>k_const_var

7. static vatiables have s_ prefix                          
>s_static_var

8. struct members are all regular names                     
>name_or_something

9. all pointers have a p_ prefix                            
>p_stack_pointer

10. all references have a r_ prefix                         
>r_reference

11. all enum members have to be uppercase                   
>NAME_OF_ENUM_MEMBER
