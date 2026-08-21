

# File SceneObjFactory.h

[**File List**](files.md) **>** [**backup**](dir_70d69dea5d1e5ae3147e3b96d60a7ce1.md) **>** [**include**](dir_e05fb92cc301336445c4f62f6c4f58b8.md) **>** [**Scene**](dir_84f8925aa2d2bbbcb80a56e59501bb98.md) **>** [**SceneObjFactory.h**](_scene_obj_factory_8h.md)

[Go to the documentation of this file](_scene_obj_factory_8h.md)


```C++
#pragma once

#include <Scene/alSceneObjHolder.h>

#define SCENE_OBJ_LIST                                                         \
  X(0, CameraDirector)                                                         \
  X(1, CameraShaker)                                                           \
  //X(2, )                                                                       \
  X(3, SwitchAreaDirector)                                                     \
  X(4, SceneAudioDirector)                                                     \
  X(5, SoundEmitAreaDirector)                                                  \
  X(6, AudioVolumeSettingAreaDirector)                                         \
  X(7, CoinRotator)                                                            \
  //X(8, )                                                                       \
  //X(9, )                                                                       \
  //X(10, )                                                                       \
  //X(11, )                                                                       \
  //X(12, )                                                                       \
  //X(13, )                                                                       \
  X(14, TimerSePlayer)                                                         \
  X(15, PlayerSceneObject)                                                     \
  X(16, BlockRailDirector)                                                     \
  X(17, PatapataWingWarp)                                                      \
  X(18, PlayerItemsStorage)                                                    \
  X(20, GhostPlayerRecorder)                                                   \
  //X(21, )                                                                       \
  X(22, GyroInputReader)

class SceneObjFactory {
public:
  static al::SceneObjHolder *createSceneObjHolder();

}; // namespace SceneObjFactory


enum SceneObjType {
#define X(i, n) SceneObj_##n = i,
    SCENE_OBJ_LIST
#undef X
    SceneObj_Max
};

```


