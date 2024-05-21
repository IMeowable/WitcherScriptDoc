#r4Game public methods

Могут быть вызваны статически через

```
theGame.Method()

```

|Функция|Описание|
| :-: | :-: |
|IsUberMovementEnabled()|Возвращает булево значение, указывающее, включено ли ускоренное движение.|
|Функция|Описание|
|IsUberMovementEnabled()|Возвращает булево значение, указывающее, включено ли ускоренное движение.|
|SetIsRespawningInLastCheckpoint()|Устанавливает флаг, что игрок возрождается на последнем контрольном пункте.|
|IsFocusModeActive()|Проверяет, активен ли режим фокуса, возвращает булево значение.|
|GetSyncAnimManager()|Возвращает экземпляр W3SyncAnimationManager, создавая его при необходимости.|
|SetEnvironmentID(id : int)|Устанавливает идентификатор окружения.|
|GetTimescaleSource(src : ETimescaleSource) : name|Возвращает имя источника изменения времени.|
|GetTimescalePriority(src : ETimescaleSource) : int|Возвращает приоритет источника изменения времени.|
|GetGamerProfile() : W3GamerProfile|Возвращает профиль игрока, инициализируя его при необходимости.|
|OnTick()|Обновляет окружение, изменяет сложность игры, если она была отложена, и обрабатывает отложенные события атаки.|
|GetCurrentZone() : EZoneName|Возвращает текущее название зоны.|
|SetCurrentZone(tag : name)|Устанавливает текущую зону по тегу.|
|GetR4ReactionManager() : CR4ReactionManager|Возвращает менеджера реакций CR4ReactionManager.|
|CreateEntity(entityTemplate : CEntityTemplate, pos : Vector, optional rot : EulerAngles, optional useAppearancesFromIncludes : bool, optional forceBehaviorPose : bool, optional doNotAdjustPlacement : bool, optional persistanceMode : EPersistanceMode, optional tagList : array< name >) : CEntity|Создает сущность на основе шаблона и других параметров.|
|GetNodeByTag(tag : name) : CNode|Возвращает узел по тегу.|
|GetEntityByTag(tag : name) : CEntity|Возвращает сущность по тегу.|
|GetEntitiesByTag(tag : name, out entities : array<CEntity>)|Возвращает массив сущностей по тегу.|
|GetNodesByTag(tag : name, out nodes : array<CNode>)|Возвращает массив узлов по тегу.|
|GetNodesByTags(tagsList : array<name>, out nodes : array<CNode>, optional matchAll : bool)|Возвращает массив узлов, соответствующих списку тегов, с возможностью задания обязательного совпадения всех тегов.|
|SetIsRespawningInLastCheckpoint()|Устанавливает флаг, что игрок возрождается на последнем контрольном пункте.|
|IsFocusModeActive()|Проверяет, активен ли режим фокуса, возвращает булево значение.|
|GetSyncAnimManager()|Возвращает экземпляр W3SyncAnimationManager, создавая его при необходимости.|
|SetEnvironmentID(id : int)|Устанавливает идентификатор окружения.|
|GetTimescaleSource(src : ETimescaleSource) : name|Возвращает имя источника изменения времени.|
|GetTimescalePriority(src : ETimescaleSource) : int|Возвращает приоритет источника изменения времени.|
|GetGamerProfile() : W3GamerProfile|Возвращает профиль игрока, инициализируя его при необходимости.|
|OnTick()|Обновляет окружение, изменяет сложность игры, если она была отложена, и обрабатывает отложенные события атаки.|
|GetCurrentZone() : EZoneName|Возвращает текущее название зоны.|
|SetCurrentZone(tag : name)|Устанавливает текущую зону по тегу.|
|GetR4ReactionManager() : CR4ReactionManager|Возвращает менеджера реакций CR4ReactionManager.|
|CreateEntity(entityTemplate : CEntityTemplate, pos : Vector, optional rot : EulerAngles, optional useAppearancesFromIncludes : bool, optional forceBehaviorPose : bool, optional doNotAdjustPlacement : bool, optional persistanceMode : EPersistanceMode, optional tagList : array< name >) : CEntity|Создает сущность на основе шаблона и других параметров.|
|GetNodeByTag(tag : name) : CNode|Возвращает узел по тегу.|
|GetEntityByTag(tag : name) : CEntity|Возвращает сущность по тегу.|
|GetEntitiesByTag(tag : name, out entities : array<CEntity>)|Возвращает массив сущностей по тегу.|
|GetNodesByTag(tag : name, out nodes : array<CNode>)|Возвращает массив узлов по тегу.|
|GetNodesByTags(tagsList : array<name>, out nodes : array<CNode>, optional matchAll : bool)|Возвращает массив узлов, соответствующих списку тегов, с возможностью задания обязательного совпадения всех тегов.|

