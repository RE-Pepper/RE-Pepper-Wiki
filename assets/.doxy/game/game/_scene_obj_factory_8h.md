

# File SceneObjFactory.h



[**FileList**](files.md) **>** [**backup**](dir_70d69dea5d1e5ae3147e3b96d60a7ce1.md) **>** [**include**](dir_e05fb92cc301336445c4f62f6c4f58b8.md) **>** [**Scene**](dir_84f8925aa2d2bbbcb80a56e59501bb98.md) **>** [**SceneObjFactory.h**](_scene_obj_factory_8h.md)

[Go to the source code of this file](_scene_obj_factory_8h_source.md)



* `#include <Scene/alSceneObjHolder.h>`















## Classes

| Type | Name |
| ---: | :--- |
| class | [**SceneObjFactory**](class_scene_obj_factory.md) <br> |


## Public Types

| Type | Name |
| ---: | :--- |
| enum  | [**SceneObjType**](#enum-sceneobjtype)  <br> |




















## Public Functions

| Type | Name |
| ---: | :--- |
|   | [**X**](#function-x) (3, SwitchAreaDirector) <br> |
|  SceneAudioDirector | [**X**](#function-x) (5, SoundEmitAreaDirector) <br> |
|  SceneAudioDirector AudioVolumeSettingAreaDirector | [**X**](#function-x) (7, CoinRotator) <br> |
|  SceneAudioDirector AudioVolumeSettingAreaDirector PlayerSceneObject | [**X**](#function-x) (16, BlockRailDirector) <br> |
|  SceneAudioDirector AudioVolumeSettingAreaDirector PlayerSceneObject PatapataWingWarp | [**X**](#function-x) (18, PlayerItemsStorage) <br> |



























## Macros

| Type | Name |
| ---: | :--- |
| define  | [**SCENE\_OBJ\_LIST**](_scene_obj_factory_8h.md#define-scene_obj_list)  `/* multi line expression */`<br> |
| define  | [**X**](_scene_obj_factory_8h.md#define-x) (i, n) `SceneObj\_##n = i,`<br> |

## Public Types Documentation




### enum SceneObjType 

```C++
enum SceneObjType {
    SceneObj_Max
};
```




<hr>
## Public Functions Documentation




### function X 

```C++
X (
    3,
    SwitchAreaDirector
) 
```




<hr>



### function X 

```C++
SceneAudioDirector X (
    5,
    SoundEmitAreaDirector
) 
```




<hr>



### function X 

```C++
SceneAudioDirector AudioVolumeSettingAreaDirector X (
    7,
    CoinRotator
) 
```




<hr>



### function X 

```C++
SceneAudioDirector AudioVolumeSettingAreaDirector PlayerSceneObject X (
    16,
    BlockRailDirector
) 
```




<hr>



### function X 

```C++
SceneAudioDirector AudioVolumeSettingAreaDirector PlayerSceneObject PatapataWingWarp X (
    18,
    PlayerItemsStorage
) 
```




<hr>
## Macro Definition Documentation





### define SCENE\_OBJ\_LIST 

```C++
#define SCENE_OBJ_LIST `X (0, CameraDirector)                                                         \ X (1, CameraShaker)                                                           \`
```




<hr>



### define X 

```C++
#define X (
    i,
    n
) `SceneObj_##n = i,`
```




<hr>

------------------------------
The documentation for this class was generated from the following file `Game/backup/include/Scene/SceneObjFactory.h`

