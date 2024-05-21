#Methods of W3PlayerWitcher

Публичные методы, которые вызываются на экземпляре объекта класса.

|Сигнатура метода|Описание|
| :-: | :-: |
|Сигнатура метода|Описание|
|GetEquippedSword(steel: bool): SItemUniqueId|Возвращает уникальный идентификатор экипированного меча в зависимости от материала (сталь или серебро).|
|OnShieldHit()|Устанавливает время жизни для эффекта удара Quen и применяет эффект триггера геймпада.|
|ApplyCastSettings()|Применяет эффект триггера геймпада для текущего экипированного знака.|
|GetSignEntity(type: ESignType): W3SignEntity|Возвращает сущность знака в зависимости от предоставленного типа знака.|
|GetSignTemplate(type: ESignType): CEntityTemplate|Возвращает шаблон знака в зависимости от предоставленного типа знака.|
|IsCurrentSignChanneled(): bool|Проверяет, происходит ли в данный момент канализация текущего знака.|
|IsCastingSign(): bool|Проверяет, происходит ли в данный момент отливка знака.|
|ProcessLockTarget(newLockTarget: CActor, checkLeftStickHeading: bool): bool|Обрабатывает блокировку цели и обновляет отображение в зависимости от типа знака.|
|PlayHitEffect(damageAction: W3DamageAction)|Воспроизводит эффекты удара в зависимости от типа и положения действия урона.|
|OnSpecialAttackHeavyActionProcess()|Сбрасывает фокусные точки на HUD во время сильного специального атакующего действия.|
|GetEnemies(): array<CActor>|Получает враждебных врагов, видимых для игрока.|
|StartCSAnim(buff: CBaseGameplayEffect): bool|Начинает анимацию боевого состояния, если под кроватью нет критического эффекта урона с течением времени под щитом Quen.|
|GetPotionBuffLevel(effectType: EEffectType): int|Получает уровень баффа зелья для заданного типа эффекта.|
|OnLevelGained(currentLevel: int, show: bool)|Обрабатывает действия при повышении уровня, такие как добавление достижений и обновление HUD.|
|GetSignStats(skill: ESkill, out damageType: name, out damageVal: float, out spellPower: SAbilityAttributeValue)|Получает статистику для заданного навыка знака, включая тип урона, значение и силу заклинания.|
|GetSkillPathType(skill: ESkill): ESkillPath|Получает тип пути навыка.|
|GetSkillLevel(s: ESkill): int|Получает уровень навыка.|
|GetSkillMaxLevel(s: ESkill): int|Получает максимальный уровень навыка.|
|GetBoughtSkillLevel(s: ESkill): int|Получает купленный уровень навыка.|
|GetAxiiLevel(): int|Получает уровень знака Axii.|
|IsInFrenzy(): bool|Проверяет, находится ли персонаж игрока в режиме безумия.|
|HasRecentlyCountered(): bool|Проверяет, был ли недавно отбит удар персонажа игрока.|
|SetRecentlyCountered(counter: bool)|Устанавливает, был ли недавно отбит удар персонажа игрока.|
|AddPoints(type: ESpendablePointType, amount: int, show: bool)|Добавляет очки для определенного типа расходных очков и обновляет отображение.|
|GetLevel(): int|Получает текущий уровень игрока.|
|GetMaxLevel(): int|Получает максимальный достижимый уровень.|
|GetTotalExpForNextLevel(): int|Получает общий опыт, необходимый для следующего уровня.|
|GetPointsTotal(type: ESpendablePointType): int|Получает общее количество очков для определенного типа расходных очков.|
|IsAutoLeveling(): bool|Проверяет, включено ли автоматическое повышение уровня.|
|SetAutoLeveling(b: bool)|Устанавливает автоматическое повышение уровня в указанное значение.|
|GetMissingExpForNextLevel(): int|Получает оставшийся опыт для следующего уровня.|
|OnSignCastPerformed(signType: ESignType, isAlternate: bool)|Обрабатывает действия после произнесения знака, такие как применение эффектов и отображение визуальных эффектов.|
|CanMeditateHere(): bool|Проверяет, можно ли медитировать в текущем месте.|
|Meditate(): bool|Инициирует медитацию, если выполнены условия.|
|MeditationRestoring(simulatedTime: float)|Обрабатывает восстановление действий во время медитации.|
|GetEquippedSword(steel: bool): SItemUniqueId|Возвращает уникальный идентификатор экипированного меча в зависимости от материала (сталь или серебро).|
|OnShieldHit()|Устанавливает время жизни для эффекта удара Quen и применяет эффект триггера геймпада.|
|ApplyCastSettings()|Применяет эффект триггера геймпада для текущего экипированного знака.|
|GetSignEntity(type: ESignType): W3SignEntity|Возвращает сущность знака в зависимости от предоставленного типа знака.|
|GetSignTemplate(type: ESignType): CEntityTemplate|Возвращает шаблон знака в зависимости от предоставленного типа знака.|
|IsCurrentSignChanneled(): bool|Проверяет, происходит ли в данный момент канализация текущего знака.|
|IsCastingSign(): bool|Проверяет, происходит ли в данный момент отливка знака.|
|ProcessLockTarget(newLockTarget: CActor, checkLeftStickHeading: bool): bool|Обрабатывает блокировку цели и обновляет отображение в зависимости от типа знака.|
|PlayHitEffect(damageAction: W3DamageAction)|Воспроизводит эффекты удара в зависимости от типа и положения действия урона.|
|OnSpecialAttackHeavyActionProcess()|Сбрасывает фокусные точки на HUD во время сильного специального атакующего действия.|
|GetEnemies(): array<CActor>|Получает враждебных врагов, видимых для игрока.|
|StartCSAnim(buff: CBaseGameplayEffect): bool|Начинает анимацию боевого состояния, если под кроватью нет критического эффекта урона с течением времени под щитом Quen.|
|GetPotionBuffLevel(effectType: EEffectType): int|Получает уровень баффа зелья для заданного типа эффекта.|
|OnLevelGained(currentLevel: int, show: bool)|Обрабатывает действия при повышении уровня, такие как добавление достижений и обновление HUD.|
|GetSignStats(skill: ESkill, out damageType: name, out damageVal: float, out spellPower: SAbilityAttributeValue)|Получает статистику для заданного навыка знака, включая тип урона, значение и силу заклинания.|
|GetSkillPathType(skill: ESkill): ESkillPath|Получает тип пути навыка.|
|GetSkillLevel(s: ESkill): int|Получает уровень навыка.|
|GetSkillMaxLevel(s: ESkill): int|Получает максимальный уровень навыка.|
|GetBoughtSkillLevel(s: ESkill): int|Получает купленный уровень навыка.|
|GetAxiiLevel(): int|Получает уровень знака Axii.|
|IsInFrenzy(): bool|Проверяет, находится ли персонаж игрока в режиме безумия.|
|HasRecentlyCountered(): bool|Проверяет, был ли недавно отбит удар персонажа игрока.|
|SetRecentlyCountered(counter: bool)|Устанавливает, был ли недавно отбит удар персонажа игрока.|
|AddPoints(type: ESpendablePointType, amount: int, show: bool)|Добавляет очки для определенного типа расходных очков и обновляет отображение.|
|GetLevel(): int|Получает текущий уровень игрока.|
|GetMaxLevel(): int|Получает максимальный достижимый уровень.|
|GetTotalExpForNextLevel(): int|Получает общий опыт, необходимый для следующего уровня.|
|GetPointsTotal(type: ESpendablePointType): int|Получает общее количество очков для определенного типа расходных очков.|
|IsAutoLeveling(): bool|Проверяет, включено ли автоматическое повышение уровня.|
|SetAutoLeveling(b: bool)|Устанавливает автоматическое повышение уровня в указанное значение.|
|GetMissingExpForNextLevel(): int|Получает оставшийся опыт для следующего уровня.|
|OnSignCastPerformed(signType: ESignType, isAlternate: bool)|Обрабатывает действия после произнесения знака, такие как применение эффектов и отображение визуальных эффектов.|
|CanMeditateHere(): bool|Проверяет, можно ли медитировать в текущем месте.|
|Meditate(): bool|Инициирует медитацию, если выполнены условия.|
|MeditationClockStart(m: CR4MeditationClockMenu)|Начинает счетчик медитации и обновляет дисплей метидации.|
|MeditationClockStop()|Останавливает счетчик медитации|
|UpdateClockTime(dt: float, id: int)|Обновляет время тиков медитации|
|SetWaitTargetHour(t: int)|Устанавливает целевой час медитации|

GetWaitTargetHour(): int	Retrieves the target hour for waiting during meditation.
MeditationForceAbort(forceCloseUI: bool)	Forces aborting meditation and handles related actions.
Runeword10Triggerred()	Handles actions triggered by Runeword 10.
Runeword12Triggerred()	Handles actions triggered by Runeword 12.
ManageSleeping()	Manages actions related to sleeping.
IsSignBlocked(signType: ESignType): bool	Checks if a sign is blocked based on the sign type.
