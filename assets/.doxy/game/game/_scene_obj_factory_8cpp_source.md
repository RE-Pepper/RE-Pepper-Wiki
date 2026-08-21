

# File SceneObjFactory.cpp

[**File List**](files.md) **>** [**backup**](dir_70d69dea5d1e5ae3147e3b96d60a7ce1.md) **>** [**src**](dir_47d28cd3eb946f860e1fe0f4e720b9c2.md) **>** [**Scene**](dir_fb9772b5c504ce2c5175abf5c52834df.md) **>** [**SceneObjFactory.cpp**](_scene_obj_factory_8cpp.md)

[Go to the documentation of this file](_scene_obj_factory_8cpp.md)


```C++
#include "SceneObjFactory.h"

al::SceneObj* createSceneObj(SceneObjType type) {
#define X(i, n) case i: return new N();
    switch case(type) {
        SCENE_OBJ_LIST
    };
#undef X
}

al::SceneObjHolder* SceneObjFactory::createSceneObjHolder() {
    return new al::SceneObjHolder(&sceneObjCreator, SceneObj_Max);
}
```


