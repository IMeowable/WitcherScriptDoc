|**Функция**|**Описание**|
| :-: | :-: |
|GetIgnoreImmortalDodge() : bool|Возвращает значение типа bool, указывающее, игнорируется ли бессмертное уклонение.|
|SetTatgetableByPlayer(isTargetAble : bool)|Устанавливает, может ли игрок выбирать этот объект в качестве цели, на основе переданного значения типа bool.|
|IsTargetableByPlayer() : bool|Проверяет, доступен ли объект для выбора игроком в качестве цели, в зависимости от текущего режима игрока и отношения объекта к игроку.|
|IsUsingTooltip() : bool|Возвращает значение типа bool, указывающее, используется ли подсказка для этого объекта.|
|SetIsUsingTooltip(hasTooltip : bool)|Устанавливает, используется ли подсказка для этого объекта, на основе переданного значения типа bool.|
|GetTotalWeaponDamage(weaponId : SItemUniqueId, damageTypeName : name, crossbowId : SItemUniqueId) : float|Возвращает общий урон оружия на основе переданных идентификаторов оружия и амуниции, а также типа урона.|
|GetAttributeValue(attributeName : name, optional tags : array<name>, optional ignoreDeath : bool) : SAbilityAttributeValue|Возвращает атрибут значения, в зависимости от переданного имени атрибута и других опциональных параметров.|
|GetAbilityAttributeValue(abilityName : name, attributeName : name) : SAbilityAttributeValue|Возвращает значение атрибута способности на основе переданных имен способности и атрибута.|
|IsAbilityBlocked(abilityName : name) : bool|Проверяет, заблокирована ли способность с указанным именем.|
|BlockAbility(abilityName : name, block : bool, optional cooldown : float) : bool|Блокирует или разблокирует способность с указанным именем на основе переданного значения block типа bool, а также устанавливает опциональный период восстановления.|
|MuteHeadAudio(mute: bool)|Импортирует функцию для отключения звука головы.|
|CanPush(canPush: bool)|Импортирует функцию, позволяющую объекту оказывать давление на другие объекты.|

|**Функция**|**Описание**|
| :-: | :-: |
|WillBeUnconscious() : bool|Проверяет, будет ли объект находиться в бессознательном состоянии.|
|IsImmortal() : bool|Проверяет, является ли объект бессмертным.|
|IsInvulnerable() : bool|Проверяет, является ли объект неуязвимым.|
|IsVulnerable() : bool|Проверяет, является ли объект уязвимым.|
|GetImmortalityMode() : EActorImmortalityMode|Возвращает текущий режим бессмертия объекта.|
|LogAllAbilities()|Журналирует все способности объекта.|
|ForceVulnerable()|Принудительно устанавливает объекту уязвимый статус.|
|ForceVulnerableImmortalityMode()|Принудительно устанавливает объекту уязвимый статус в режиме бессмертия.|
|RestoreImmortalityMode()|Восстанавливает режим бессмертия объекта.|
|GetImmortalityModeChannels(mode : EActorImmortalityMode) : array< EActorImmortalityChanel >|Возвращает массив каналов режима бессмертия объекта для заданного режима.|
|SetImmortalityMode(mode : EActorImmortalityMode, channel : EActorImmortalityChanel, optional lockMode : bool)|Устанавливает режим бессмертия объекта для заданного канала и опционально блокирует изменение этого режима.|

|**Функция**|**Описание**|
| :-: | :-: |
|IsInCombat() : bool|Проверяет, находится ли объект в бою.|
|SetCombatStartTime()|Устанавливает время начала боя для объекта.|
|GetCombatStartTime() : float|Получает время начала текущего боя объекта.|
|ResetCombatStartTime()|Сбрасывает время начала текущего боя объекта.|
|SetCombatPartStartTime()|Устанавливает время начала текущей части боя объекта.|
|ResetCombatPartStartTime()|Сбрасывает время начала текущей части боя объекта.|
|GetCombatTime() : float|Получает время, проведенное в текущем бою.|
|GetCombatPartTime() : float|Получает время, проведенное в текущей части боя.|
|HasHitTarget() : bool|Проверяет, попал ли объект в цель.|
|WasDefeatedFromFistFight() : bool|Проверяет, был ли объект побежден в драке кулачным боем.|
|event OnStartFistfightMinigame()|Событие, вызываемое при начале мини-игры в драку кулачным боем.|
|event OnEndFistfightMinigame()|Событие, вызываемое при завершении мини-игры в драку кулачным боем.|
|IsInFistFightMiniGame() : bool|Проверяет, находится ли объект в режиме мини-игры в драку кулачным боем.|

|**Функция**|**Описание**|
| :-: | :-: |
|IsInAir() : bool|Проверяет, находится ли объект в воздухе.|
|SetIsInAir(b : bool)|Устанавливает состояние объекта в воздухе.|
|GetRagdollPullingStartPosition() : Vector|Получает начальную позицию для тяги куклы объекта.|
|event OnRagdollPullingStarts(ragdollPos, entityPos : Vector)|Событие, вызываемое при начале тяги куклы объекта.|
|IsInCutsceneIntro() : bool|Проверяет, находится ли объект во время вступительной сцены (интро).|
|SetIsInCutsceneIntro(b : bool)|Устанавливает состояние объекта во время вступительной сцены (интро).|

|**Функция**|**Описание**|
| :-: | :-: |
|ActionMoveToNode(target : CNode, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Перемещает объект к указанной узловой точке.|
|ActionMoveToNodeAsync(target : CNode, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Асинхронно перемещает объект к указанной узловой точке.|
|ActionMoveToNodeWithHeading(target : CNode, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Перемещает объект к указанной узловой точке с учетом направления.|
|ActionMoveToNodeWithHeadingAsync(target : CNode, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Асинхронно перемещает объект к указанной узловой точке с учетом направления.|
|ActionMoveTo(target : Vector, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Перемещает объект к указанной точке в пространстве.|
|ActionMoveToAsync(target : Vector, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Асинхронно перемещает объект к указанной точке в пространстве.|
|ActionMoveToWithHeading(target : Vector, heading : float, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Перемещает объект к указанной точке в пространстве с учетом направления.|
|ActionMoveToWithHeadingAsync(target : Vector, heading : float, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Асинхронно перемещает объект к указанной точке в пространстве с учетом направления.|
|ActionMoveToDynamicNode(target : CNode, moveType : EMoveType, absSpeed : float, range : float, optional keepDistance : bool, optional failureAction : EMoveFailureAction) : bool|Перемещает объект к указанной динамической узловой точке.|
|ActionMoveToDynamicNodeAsync(target : CNode, moveType : EMoveType, absSpeed : float, range : float, optional keepDistance : bool, optional failureAction : EMoveFailureAction) : bool|Асинхронно перемещает объект к указанной динамической узловой точке.|
|ActionMoveCustom(targeter : CMoveTRGScript) : bool|Выполняет пользовательское движение по целевому скрипту движения.|
|ActionMoveCustomAsync(targeter : CMoveTRGScript) : bool|Асинхронно выполняет пользовательское движение по целевому скрипту движения.|
|ActionSlideThrough(explorationAreaToUse : CActionAreaComponent) : bool|Производит скольжение через указанную область действия.|
|ActionSlideThroughAsync(explorationAreaToUse : CActionAreaComponent) : bool|Асинхронно производит скольжение через указанную область действия.|
|ActionSlideTo(target : Vector, duration : float) : bool|Скольжение к указанной точке в пространстве за указанное время.|
|ActionSlideToAsync(target : Vector, duration : float) : bool|Асинхронное скольжение к указанной точке в пространстве за указанное время.|
|ActionMoveOnCurveTo(target : Vector, duration : float, rightShift : bool) : bool|Движение по кривой к указанной точке за указанное время.|
|ActionMoveOnCurveToAsync(target : Vector, duration : float, rightShift : bool) : bool|Асинхронное движение по кривой к указанной точке за указанное время.|
|ActionSlideToWithHeading(target : Vector, heading : float, duration : float, optional rotation : ESlideRotation) : bool|Скольжение к указанной точке в пространстве с учетом направления за указанное время.|
|ActionSlideToWithHeadingAsync(target : Vector, heading : float, duration : float, optional rotation : ESlideRotation) : bool|Асинхронное скольжение к указанной точке в пространстве с учетом направления за указанное время.|
|ActionMoveAwayFromNode(position : CNode, distance : float, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Отходит от указанной узловой точки на заданное расстояние.|
|ActionMoveAwayFromNodeAsync(position : CNode, distance : float, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Асинхронно отходит от указанной узловой точки на заданное расстояние.|
|ActionMoveAwayFromLine(positionA : Vector, positionB : Vector, distance : float, makeMinimalMovement : bool, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Отходит от указанной линии на заданное расстояние.|
|`ActionMoveAwayFromLineAsync(positionA : Vector, positionB : Vector, distance : float||

|**Функция**|**Описание**|
| :-: | :-: |
|ActionMoveAwayFromLine(positionA : Vector, positionB : Vector, distance : float, makeMinimalMovement : bool, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Отходит от указанной линии на заданное расстояние.|
|ActionMoveAwayFromLineAsync(positionA : Vector, positionB : Vector, distance : float, makeMinimalMovement : bool, optional moveType : EMoveType, optional absSpeed : float, optional radius : float, optional failureAction : EMoveFailureAction) : bool|Асинхронно отходит от указанной линии на заданное расстояние.|
|ActionRotateTo(target : Vector) : bool|Поворачивает объект к указанной точке в пространстве.|
|ActionRotateToAsync(target : Vector) : bool|Асинхронно поворачивает объект к указанной точке в пространстве.|
|ActionSetOrientation(orientation : float) : bool|Устанавливает ориентацию объекта в пространстве.|
|ActionPlaySlotAnimation(slotName : name, animationName : name, optional blendIn : float, optional blendOut : float, optional continuePlaying : bool) : bool|Воспроизводит анимацию в указанном слоте.|
|ActionPlaySlotAnimationAsync(slotName : name, animationName : name, optional blendIn : float, optional blendOut : float, optional continuePlaying : bool) : bool|Асинхронно воспроизводит анимацию в указанном слоте.|
|ActionExitWork(optional fast : bool) : bool|Завершает текущую работу.|
|ActionExitWorkAsync(optional fast : bool) : bool|Асинхронно завершает текущую работу.|

|**Функция**|**Описание**|
| :-: | :-: |
|IsAlive() : bool|Проверяет, жив ли объект.|
|Heal(amount : float)|Лечит объект на указанное количество единиц здоровья.|
|SetHealthPerc(amount : float)|Устанавливает здоровье объекта в процентах от максимального значения.|
|SetHealth(amount : float)|Устанавливает здоровье объекта в указанное количество единиц.|

|**Функция**|**Описание**|
| :-: | :-: |
|SetAlive(flag : bool)|Устанавливает состояние живучести объекта.|
|IsExternalyControlled() : bool|Проверяет, управляется ли объект внешне.|
|IsMoving() : bool|Проверяет, двигается ли объект.|
|GetMoveDestination() : Vector|Возвращает позицию, к которой объект движется.|
|GetPositionOrMoveDestination() : Vector|Возвращает текущую позицию объекта или позицию, к которой он движется.|
|GetVoicetag() : name|Возвращает метку голоса объекта.|
|EnableCollisions(val : bool)|Включает или выключает коллизии для объекта.|
|PredictWorldPosition(inTime : float) : Vector|Предсказывает позицию объекта в мире через указанное время.|
|GetHeadAngleHorizontal() : float|Возвращает горизонтальный угол головы объекта.|
|GetHeadAngleVertical() : float|Возвращает вертикальный угол головы объекта.|
|GetMovingAgentComponent() : CMovingAgentComponent|Получает компонент, управляющий движением объекта.|
|GetMorphedMeshManagerComponent() : CMorphedMeshManagerComponent|Получает компонент, управляющий морфингом меша объекта.|
|EnablePathEngineAgent(flag : bool)|Включает или выключает агент пути объекта.|
|EnableCollisionInfoReportingForItem(itemId : SItemUniqueId, enable : bool)|Включает или выключает отчет о коллизиях для указанного элемента.|
|EnablePhysicalMovement(enable : bool) : bool|Включает или выключает физическое перемещение объекта.|
|EnableStaticCollisions(enable : bool) : bool|Включает или выключает статические коллизии объекта.|
|EnableDynamicCollisions(enable : bool) : bool|Включает или выключает динамические коллизии объекта.|
|EnableCharacterCollisions(enable : bool) : bool|Включает или выключает коллизии объекта с персонажем.|
|PushInDirection(pusherPos : Vector, direction : Vector, optional speed : float, optional playAnimation : bool, optional applyRotation : bool)|Толкает объект в указанном направлении от указанной позиции.|
|PushAway(pusher : CMovingAgentComponent, optional strength : float, optional speed : float)|Отталкивает объект от другого объекта с учетом силы и скорости.|
|IsRagdollObstacle() : bool|Проверяет, является ли объект препятствием для ригидного тела (ragdoll).|
|ForceAIBehavior(tree : IAITree, forceLevel : EArbitratorPriorities, optional forceEventName : name) : int|Принудительно активирует поведение ИИ с указанным приоритетом.|
|CancelAIBehavior(forceActionId : int) : bool|Отменяет принудительное активированное действие ИИ.|
|IsFrozen() : bool|Проверяет, заморожен ли объект.|

|**Функция**|**Описание**|
| :-: | :-: |
|SetAlive(flag: bool)|Устанавливает состояние живучести персонажа.|
|IsExternalyControlled(): bool|Проверяет, управляется ли персонаж внешним образом.|
|IsMoving(): bool|Проверяет, перемещается ли персонаж в данный момент.|
|GetMoveDestination(): Vector|Получает вектор назначения для перемещения персонажа.|
|GetPositionOrMoveDestination(): Vector|Получает позицию или вектор назначения перемещения персонажа.|
|GetVoicetag(): name|Получает тег голоса персонажа.|
|EnableCollisions(val: bool)|Включает или выключает коллизии для персонажа.|
|PredictWorldPosition(inTime: float): Vector|Предсказывает мировую позицию персонажа на основе заданного времени в будущем.|
|GetHeadAngleHorizontal(): float|Получает горизонтальный угол наклона головы персонажа.|
|GetHeadAngleVertical(): float|Получает вертикальный угол наклона головы персонажа.|
|GetMovingAgentComponent(): CMovingAgentComponent|Получает компонент движения персонажа.|

|**Функция**|**Описание**|
| :-: | :-: |
|IsOnGround(): bool|Проверяет, находится ли персонаж на земле.|
|IsFalling(): bool|Проверяет, падает ли персонаж.|
|GetDistanceFromGround(\_MaxTestDistance: float, optional \_CollisionGroupNames: array<name>): float|Получает расстояние от персонажа до земли.|
|IsAttackableByPlayer(): bool|Проверяет, может ли персонаж быть атакован игроком.|
|SetAttackableByPlayerPersistent(flag: bool)|Устанавливает персонажу возможность быть атакованным игроком на протяжении всего времени жизни.|
|SetAttackableByPlayerRuntime(flag: bool, optional timeout: float)|Устанавливает персонажу возможность быть атакованным игроком на указанное время.|
|SetAnimationTimeMultiplier(mult: float)|Устанавливает множитель времени анимации.|
|SetAnimationSpeedMultiplier(mul: float, optional overrideExistingId: int): int|Устанавливает множитель скорости анимации.|
|ResetAnimationSpeedMultiplier(id: int)|Сбрасывает множитель скорости анимации по указанному идентификатору.|
|ClearAnimationSpeedMultipliers()|Очищает все множители скорости анимации.|
|GetAttackableNPCsAndPlayersInRange(range: float, optional maxResults: int, optional tag: name): array <CActor>|Получает массив атакуемых NPC и игроков в указанном радиусе.|
|GetNPCsAndPlayersInRange(range: float, optional maxResults: int, optional tag: name, optional queryFlags: int): array <CActor>|Получает массив NPC и игроков в указанном радиусе с заданными флагами запроса.|
|GetAttackableNPCsAndPlayersInCone(range: float, coneDir: float, coneAngle: float, optional maxResults: int, optional tag: name): array <CActor>|Получает массив атакуемых NPC и игроков в конусе.|
|GetNPCsAndPlayersInCone(range: float, coneDir: float, coneAngle: float, optional maxResults: int, optional tag: name, optional queryFlags: int): array <CActor>|Получает массив NPC и игроков в конусе с заданными флагами запроса.|
|IsHuman(): bool|Проверяет, является ли персонаж человеком.|
|IsWoman(): bool|Проверяет, является ли персонаж женщиной.|
|IsMan(): bool|Проверяет, является ли персонаж мужчиной.|
|IsMonster(): bool|Проверяет, является ли персонаж монстром.|
|IsAnimal(): bool|Проверяет, является ли персонаж животным.|
|IsVampire(): bool|Проверяет, является ли персонаж вампиром.|
|HasStaminaToParry(attActionName: name): bool|Проверяет, есть ли у персонажа достаточно выносливости для парирования.|
|CanParryAttack(): bool|Проверяет, может ли персонаж парировать атаку.|
|CanCounterParryAttack(attActionName: name): bool|Проверяет, может ли персонаж контратаковать после парирования атаки.|
|FistFightCheck(target, attacker: CActor, out bothUsingFists: bool): bool|Проверяет, идет ли драка кулаками между целью и атакующим.|
|ProcessSwordOrFistHitReaction(target, attacker: CActor): float|Обрабатывает реакцию на удар мечом или кулаком.|
|IsWeaponHeld(itemCategory: name): bool|Проверяет, держит ли персонаж оружие указанной категории.|
|IsAnyWeaponHeld(): bool|Проверяет, держит ли персонаж какое-либо оружие.|
|IsSecondaryWeaponHeld(): bool|Проверяет, держит ли персонаж вторичное оружие.|
|IsSwordWooden(): bool|Проверяет, является ли меч, который держит персонаж, деревянным.|
|IsDeadlySwordHeld(): bool|Проверяет, держит ли персонаж|

|**Функция**|**Описание**|
| :-: | :-: |
|SetIsCurrentlyDodging(b: bool, isRolling: bool)|Устанавливает флаг, указывающий, уклоняется ли персонаж в данный момент. Также запускает событие реакции в менеджере дерева поведения.|
|IsCurrentlyDodging(): bool|Возвращает булево значение, указывающее, уклоняется ли персонаж в данный момент.|
|SetParryEnabled(flag: bool)|Устанавливает флаг, указывающий, разрешено ли парирование.|
|GetLastAttackRangeName(): name|Возвращает имя последнего диапазона атаки.|
|CanPerformCounter(): bool|Возвращает булево значение, указывающее, может ли персонаж совершить контрудар.|
|IsGuarded(): bool|Возвращает булево значение, указывающее, находится ли персонаж под защитой.|
|SetGuarded(flag: bool)|Устанавливает состояние защиты персонажа. Если переходит из защищенного в незащищенное состояние, записывает время.|
|CanGuard(): bool|Возвращает булево значение, указывающее, может ли персонаж защищаться на основе условия задержки.|
|DisableHitAnimFor(time: float)|Отключает анимацию удара на определенное время.|
|UseAdditiveHit(): bool|Возвращает булево значение, указывающее, используется ли дополнительный удар.|
|SetUseAdditiveHit(\_Flag: bool, \_CriticalCancelAdditiveHit: bool, \_OneTimeActivation: bool)|Устанавливает использование дополнительного удара с возможностью критической отмены. Параметр \_OneTimeActivation используется для однократной активации.|
|UseAdditiveCriticalState(): bool|Возвращает булево значение, указывающее, используется ли дополнительное критическое состояние анимации.|
|SetUseAdditiveCriticalStateAnim(flag: bool)|Устанавливает использование дополнительного критического состояния анимации.|
|SetCanPlayHitAnim(flag: bool)|Устанавливает возможность воспроизведения анимации удара.|
|CanPlayHitAnim(): bool|Возвращает булево значение, указывающее, может ли воспроизводиться анимация удара.|
|StopRotateEventAdjustments()|Останавливает корректировки событий вращения.|
|GetCriticalCancelAdditiveHit(): bool|Возвращает булево значение, указывающее, может ли быть отменен дополнительный удар.|
|GetAbilityManager(): W3AbilityManager|Возвращает менеджер способностей.|


|**Функция**|**Описание**|
| :-: | :-: |
|IsDeadlySwordHeld(): bool|Проверяет, держит ли персонаж смертоносный меч. Возвращает true, если не держит деревянный меч, не держит вторичное оружие и не держит кулаки.|
|DrainStamina(action: EStaminaActionType, fixedCost: float, fixedDelay: float, abilityName: name, dt: float, costMult: float)|Отнимает выносливость в зависимости от действия.|
|DrainAir(cost: float, regenDelay: float)|Отнимает воздух.|
|DrainSwimmingStamina(cost: float, regenDelay: float)|Отнимает выносливость при плавании.|
|DrainMorale(amount: float)|Отнимает мораль.|
|DrainVitality(amount: float)|Отнимает жизненную силу.|
|DrainEssence(amount: float)|Отнимает сущность.|
|AddPanic(amount: float)|Добавляет панику.|
|GainStat(stat: EBaseCharacterStats, amount: float)|Увеличивает статистику.|
|UpdateStatMax(stat: EBaseCharacterStats)|Обновляет максимальное значение статистики.|
|ForceSetStat(stat: EBaseCharacterStats, val: float)|Принудительно устанавливает значение статистики.|
|GetPowerStatValue(stat: ECharacterPowerStats, abilityName: name, ignoreDeath: bool): SAbilityAttributeValue|Возвращает значение силы персонажа.|
|GetResistValue(stat: ECharacterDefenseStats, out points: float, out percents: float)|Получает сопротивление.|
|ResumeEffects(type: EEffectType, sourceName: name)|Возобновляет эффекты.|
|PauseEffects(type: EEffectType, sourceName: name, singleLock: bool, duration: float, useMaxDuration: bool)|Приостанавливает эффекты.|
|HasDefaultAbilitySet(): bool|Проверяет наличие стандартного набора способностей.|
|IgnoresDifficultySettings(): bool|Проверяет, игнорирует ли персонаж настройки сложности.|
|HasStaminaToUseAction(action: EStaminaActionType, abilityName: name, dt: float, multiplier: float): bool|Проверяет, есть ли у персонажа достаточно выносливости для совершения действия.|
|GetStaminaActionCost(action: EStaminaActionType, abilityName: name, dt: float): float|Получает стоимость действия в выносливости.|
|GetStaminaActionDelay(action: EStaminaActionType, abilityName: name, dt: float): float|Получает задержку действия в выносливости.|
|GetHealthPercents(): float|Получает процент здоровья.|
|GetHealth(): float|Получает значение здоровья.|
|GetStaminaPercents(): float|Получает процент выносливости.|
|GetMaxHealth(): float|Получает максимальное значение здоровья.|
|GetCurrentHealth(): float|Получает текущее значение здоровья.|
|UsesVitality(): bool|Проверяет, использует ли персонаж жизненную силу.|
|UsesEssence(): bool|Проверяет, использует ли персонаж сущность.|
|GetUsedHealthType(): EBaseCharacterStats|Получает используемый тип здоровья.|
|GetStat(stat: EBaseCharacterStats, ignoreLock: bool): float|Получает значение статистики.|
|GetStatMax(stat: EBaseCharacterStats): float|Получает максимальное значение статистики.|
|GetStats(stat: EBaseCharacterStats, curr: float, max: float)|Получает текущее и максимальное значение статистики.|
|GetStatPercents(stat: EBaseCharacterStats): float|Получает процент статистики.|

|**Функция**|**Описание**|
| :-: | :-: |
|Revive()|Воскрешает персонажа, если он мёртв, но не потерял сознание.|
|ApplyActionEffects(action: W3DamageAction): bool|Применяет эффекты действия.|
|GetHitCounter(total: bool): int|Получает счётчик ударов. Если total равен true, возвращает общее количество ударов, в противном случае — текущее.|
|IncHitCounter()|Увеличивает счётчик ударов.|
|ResetHitCounter(deta: float, id: int)|Сбрасывает счётчик ударов.|
|GetDefendCounter(total: bool): int|Получает счётчик защиты. Если total равен true, возвращает общее количество защит, в противном случае — текущее.|
|IncDefendCounter()|Увеличивает счётчик защиты.|
|ResetDefendCounter(deta: float, id: int)|Сбрасывает счётчик защиты.|
|ReactToReflectedAttack(target: CGameplayEntity)|Реакция на отражённую атаку.|
|ReactToBeingHit(damageAction: W3DamageAction, buffNotApplied: bool): bool|Реакция на получение урона.|

|**Функция**|**Описание**|
| :-: | :-: |
|PlayHitEffect(damageAction: W3DamageAction)|Воспроизводит эффект удара.|
|StartVitalityRegen(): bool|Запускает регенерацию жизненных сил.|
|StopVitalityRegen()|Останавливает регенерацию жизненных сил.|
|StartEssenceRegen(): bool|Запускает регенерацию сущности.|
|StopEssenceRegen()|Останавливает регенерацию сущности.|
|StartStaminaRegen(): bool|Запускает регенерацию выносливости.|
|StopStaminaRegen()|Останавливает регенерацию выносливости.|
|StartMoraleRegen(): bool|Запускает регенерацию боевого духа.|
|StopMoraleRegen()|Останавливает регенерацию боевого духа.|
|StartPanicRegen(): bool|Запускает регенерацию паники.|
|StopPanicRegen()|Останавливает регенерацию паники.|
|StartAirRegen(): bool|Запускает регенерацию воздуха (для подводных персонажей).|
|StopAirRegen()|Останавливает регенерацию воздуха.|
|StartSwimmingStaminaRegen(): bool|Запускает регенерацию выносливости при плавании.|
|StopSwimmingStaminaRegen()|Останавливает регенерацию выносливости при плавании.|
|GetNewRequestedCS(): CBaseGameplayEffect|Получает новое запрошенное критическое состояние.|
|SetNewRequestedCS(buff: CBaseGameplayEffect)|Устанавливает новое запрошенное критическое состояние.|
|StartCSAnim(buff: CBaseGameplayEffect): bool|Запускает анимацию критического состояния.|
|AddEffectCustom(params: SCustomEffectParams): EEffectInteract|Добавляет пользовательский эффект.|
|AddEffectDefault(effectType: EEffectType, creat: CGameplayEntity, srcName: string, signEffect: bool): EEffectInteract|Добавляет стандартный эффект.|
|ProcessOnHitEffects(victim: CActor, silverSword: bool, steelSword: bool, sign: bool)|Обрабатывает эффекты при попадании.|
|RemoveBuff(effectType: EEffectType, csForcedRemove: bool, sourceName: string)|Удаляет бафф определённого типа.|
|RemoveEffect(effect: CBaseGameplayEffect, csForcedRemove: bool)|Удаляет эффект.|
|RemoveAllNonAutoBuffs(removeOils: bool, skipPerk14: bool)|Удаляет все неавтоматические баффы.|
|RemoveAllBuffsOfType(effectType: EEffectType)|Удаляет все баффы определённого типа.|
|RemoveAllBuffsWithSource(source: string)|Удаляет все баффы с определённым источником.|
|HasBuff(effectType: EEffectType): bool|Проверяет, есть ли бафф определённого типа.|
|GetBuffTimePercentageByType(effectType: EEffectType): int|Получает процент времени баффа по типу.|
|GetBuffTimePercentage(effect: CBaseGameplayEffect): int|Получает процент времени для определённого баффа.|
|GetCriticalBuffsCount(): int|Получает количество критических баффов.|
|GetCurrentlyAnimatedCS(): CBaseGameplayEffect|Получает текущее анимированное критическое состояние.|
|GetBuff(effectType: EEffectType, sourceName: string): CBaseGameplayEffect|Получает бафф определённого типа с указанным источником.|
|GetBuffs(type: EEffectType, sourceName: string, partialSourceNameSearch: bool): array<CBaseGameplayEffect>|Получает массив баффов определённого типа с указанным источником.|

|**Функция**|**Описание**|
| :-: | :-: |
|PlayHitEffect(damageAction: W3DamageAction)|Воспроизводит эффект удара.|
|StartVitalityRegen(): bool|Запускает регенерацию жизненных сил.|
|StopVitalityRegen()|Останавливает регенерацию жизненных сил.|
|StartEssenceRegen(): bool|Запускает регенерацию сущности.|
|StopEssenceRegen()|Останавливает регенерацию сущности.|
|StartStaminaRegen(): bool|Запускает регенерацию выносливости.|
|StopStaminaRegen()|Останавливает регенерацию выносливости.|
|StartMoraleRegen(): bool|Запускает регенерацию боевого духа.|
|StopMoraleRegen()|Останавливает регенерацию боевого духа.|
|StartPanicRegen(): bool|Запускает регенерацию паники.|
|StopPanicRegen()|Останавливает регенерацию паники.|
|StartAirRegen(): bool|Запускает регенерацию воздуха (для подводных персонажей).|
|StopAirRegen()|Останавливает регенерацию воздуха.|
|StartSwimmingStaminaRegen(): bool|Запускает регенерацию выносливости при плавании.|
|StopSwimmingStaminaRegen()|Останавливает регенерацию выносливости при плавании.|
|GetNewRequestedCS(): CBaseGameplayEffect|Получает новое запрошенное критическое состояние.|
|SetNewRequestedCS(buff: CBaseGameplayEffect)|Устанавливает новое запрошенное критическое состояние.|
|StartCSAnim(buff: CBaseGameplayEffect): bool|Запускает анимацию критического состояния.|
|AddEffectCustom(params: SCustomEffectParams): EEffectInteract|Добавляет пользовательский эффект.|
|AddEffectDefault(effectType: EEffectType, creat: CGameplayEntity, srcName: string, signEffect: bool): EEffectInteract|Добавляет стандартный эффект.|
|ProcessOnHitEffects(victim: CActor, silverSword: bool, steelSword: bool, sign: bool)|Обрабатывает эффекты при попадании.|
|RemoveBuff(effectType: EEffectType, csForcedRemove: bool, sourceName: string)|Удаляет бафф определённого типа.|
|RemoveEffect(effect: CBaseGameplayEffect, csForcedRemove: bool)|Удаляет эффект.|
|RemoveAllNonAutoBuffs(removeOils: bool, skipPerk14: bool)|Удаляет все неавтоматические баффы.|
|RemoveAllBuffsOfType(effectType: EEffectType)|Удаляет все баффы определённого типа.|
|RemoveAllBuffsWithSource(source: string)|Удаляет все баффы с определённым источником.|
|HasBuff(effectType: EEffectType): bool|Проверяет, есть ли бафф определённого типа.|
|GetBuffTimePercentageByType(effectType: EEffectType): int|Получает процент времени баффа по типу.|
|GetBuffTimePercentage(effect: CBaseGameplayEffect): int|Получает процент времени для определённого баффа.|
|GetCriticalBuffsCount(): int|Получает количество критических баффов.|
|GetCurrentlyAnimatedCS(): CBaseGameplayEffect|Получает текущее анимированное критическое состояние.|
|GetBuff(effectType: EEffectType, sourceName: string): CBaseGameplayEffect|Получает бафф определённого типа с указанным источником.|
|GetBuffs(type: EEffectType, sourceName: string, partialSourceNameSearch: bool): array<CBaseGameplayEffect>|Получает массив баффов определённого типа с указанным источником.|
|AddBuffImmunity\_AllCritical(source: name, removeIfPresent: bool)|Добавляет иммунитет ко всем критическим баффам.|
|AddBuffImmunity\_AllNegative(source: name, removeIfPresent: bool)|Добавляет иммунитет ко всем негативным баффам.|
|AddBuffImmunity(effect: EEffectType, source: name, removeBuffIfPresent: bool)|Добавляет иммунитет к определённому баффу.|
|RemoveBuffImmunity\_AllCritical(source: name)|Удаляет иммунитет ко всем критическим баффам.|
|RemoveBuffImmunity\_AllNegative(source: name)|Удаляет иммунитет ко всем негативным баффам.|
|RemoveBuffImmunity(effect: EEffectType, source: name)|Удаляет иммунитет к определённому баффу.|
|SetIsRecoveringFromKnockdown()|Устанавливает флаг восстановления от нокдауна.|
|GetIsRecoveringFromKnockdown(): bool|Проверяет, восстанавливается ли персонаж от нокдауна.|
|PauseHPRegenEffects(sourceName: name, duration: float)|Приостанавливает регенерацию здоровья.|
|ResumeHPRegenEffects(sourceName: name, forceAll: bool)|Возобновляет регенерацию здоровья.|
|PauseStaminaRegen(sourceName: name, duration: float)|Приостанавливает регенерацию выносливости.|
|ResumeStaminaRegen(sourceName: name)|Возобновляет регенерацию выносливости.|
|GetCriticalStateCounter(total: bool): int|Получает количество критических состояний.|
|IncCriticalStateCounter()|Увеличивает счётчик критических состояний.|
|ResetCriticalStateCounter(deta: float, id: int)|Сбрасывает счётчик критических состояний.|
|GetTotalSignSpellPower(signSkill: ESkill): SAbilityAttributeValue|Получает общую силу знака.|
|EnableHighlightTimer(time: float, id: int)|Включает таймер подсветки.|
|SetBIsPlayerCurrentTarget(flag: bool)|Устанавливает флаг текущей цели игрока.|
|SetWound(woundName: name, spawnEntity: bool, createParticles: bool, dropEquipment: bool, playSound: bool, direction: Vector, playedEffectsMask: int)|Устанавливает рану.|
|IsCurrentWound(woundName: name): bool|Проверяет, является ли указанная рана текущей.|
|IsWoundDefined(woundName: name): bool|Проверяет, определена ли указанная рана.|
|GetNearestWoundForBone(boneIndex: int, directionWS: Vector, woundTypeFlags: EWoundTypeFlags): name|Получает ближайшую рану для кости.|
|SetDismembermentInfo(woundName: name, vec: Vector, forceRagoll: bool, playedEffectsMask: int)|Устанавливает информацию о расчленении.|
|DelayedDismemberTimer(time: float, id: int)|Запускает таймер отложенного расчленения.|
|IsSuperHeavyAttack(attackName: name): bool|Проверяет, является ли атака супер тяжёлой.|
|IsHeavyAttack(attackName: name): bool|Проверяет, является ли атака тяжёлой.|
|IsLightAttack(attackName: name): bool|Проверяет, является ли атака лёгкой.|

|**Метод**|**Описание**|||||
| :-: | :-: | :- | :- | :- | :- |
|SetWound(woundName, ...)|Устанавливает видимое ранение с указанным именем. Может создавать частицы, воспроизводить звук и т. д.|||||
|IsCurrentWound(woundName)|Проверяет, является ли указанное ранение текущим видимым ранением.|||||
|IsWoundDefined(woundName)|Проверяет, определено ли указанное ранение.|||||
|GetNearestWoundForBone(boneIndex, ...)|Возвращает ближайшее ранение к указанной кости с учетом направления и типа ранения.|||||
|SetDismembermentInfo(woundName, ...)|Устанавливает информацию о рассечении для указанного ранения.|||||
|DelayedDismemberTimer(time, id)|Таймер, который вызывает функцию Dismember через указанное время.|||||
|IsSuperHeavyAttack(attackName)|Проверяет, является ли указанная атака супертяжелой.|||||
|IsHeavyAttack(attackName)|Проверяет, является ли указанная атака тяжелой.|||||
|IsLightAttack(attackName)|Проверяет, является ли указанная атака легкой.|||||
|ReduceDamage(damageData)|Уменьшает урон, полученный от атаки, с учетом различных факторов, таких как защита, типы урона и способности персонажа.|||||
|GetDelaySinceLastAttacked()|Возвращает время, прошедшее с момента последней атаки.|||||
|**Метод**|**Сигнатура**|**Аргументы**|**Описание**|||
|SetWound|public function SetWound(woundName: name, optional spawnEntity: bool, optional createParticles: bool, optional dropEquipment: bool, optional playSound: bool, optional direction: Vector, optional playedEffectsMask: int)|woundName: имя раны <br> spawnEntity: флаг для создания сущности (необязательно) <br> createParticles: флаг для создания частиц (необязательно) <br> dropEquipment: флаг для сброса снаряжения (необязательно) <br> playSound: флаг для воспроизведения звука (необязательно) <br> direction: вектор направления (необязательно) <br> playedEffectsMask: маска воспроизведенных эффектов (необязательно)|Устанавливает рану с указанным именем с опциональными параметрами для создания эффектов, воспроизведения звуков и т.д.|||
|IsCurrentWound|public function IsCurrentWound(woundName: name) : bool|woundName: имя раны|Проверяет, является ли указанная рана текущей.|||
|IsWoundDefined|public function IsWoundDefined(woundName: name) : bool|woundName: имя раны|Проверяет, определена ли указанная рана.|||
|GetNearestWoundForBone|public function GetNearestWoundForBone(boneIndex: int, directionWS: Vector, woundTypeFlags: EWoundTypeFlags) : name|boneIndex: индекс кости <br> directionWS: вектор направления мира <br> woundTypeFlags: флаги типа раны|Получает ближайшую рану для указанной кости с определенными флагами типа раны.|||
|SetDismembermentInfo|public function SetDismembermentInfo(woundName: name, vec: Vector, forceRagoll: bool, optional playedEffectsMask: int)|woundName: имя раны <br> vec: вектор <br> forceRagoll: флаг для регулировки уровня регдолла <br> playedEffectsMask: маска воспроизведенных эффектов (необязательно)|Устанавливает информацию о демонтировании с указанным именем раны и опциональными параметрами.|||
|DelayedDismemberTimer|public timer function DelayedDismemberTimer(time: float, id: int)|time: время <br> id: идентификатор|Запускает таймер для отложенного демонтирования.|||
|IsSuperHeavyAttack|public function IsSuperHeavyAttack(attackName: name) : bool|attackName: имя атаки|Проверяет, является ли указанная атака супертяжелой.|||
|IsHeavyAttack|public function IsHeavyAttack(attackName: name) : bool|attackName: имя атаки|Проверяет, является ли указанная атака тяжелой.|||
|IsLightAttack|public function IsLightAttack(attackName: name) : bool|attackName: имя атаки|Проверяет, является ли указанная атака легкой.|||
|ReduceDamage|public function ReduceDamage(out damageData: W3DamageAction)|damageData: данные о повреждениях|Уменьшает урон, нанесенный указанным действием.|||
|GetDelaySinceLastAttacked|public function GetDelaySinceLastAttacked() : float|-|Получает задержку с момента последней атаки.|||

|**Метод**|**Сигнатура**|**Аргументы**|**Описание**|
| :-: | :-: | :-: | :-: |
|GetDelaySinceLastHit|public function GetDelaySinceLastHit() : float|-|Получает задержку с момента последнего удара.|
|IsAttacked|public function IsAttacked(optional byPlayer: bool) : void|byPlayer: флаг, указывающий, был ли атакован игроком (необязательно)|Регистрирует атаку на объекте, устанавливает время последней атаки. Если атаковал игрок, генерирует событие "AttackedByPlayer".|
|IsAttackerAtBack|function IsAttackerAtBack(attacker: CNode) : bool|attacker: атакующий объект|Проверяет, находится ли атакующий объект сзади данного объекта.|
|GetTotalArmor|public function GetTotalArmor() : SAbilityAttributeValue|-|Получает общее значение брони.|


