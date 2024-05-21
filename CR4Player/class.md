|Метод|Назначение|Параметры|Возвращаемое значение|
| :-: | :-: | :-: | :-: |
|Метод|Назначение|Параметры|Возвращаемое значение|
|SetShowToLowStaminaIndication|Устанавливает значение индикатора низкой выносливости|value: float|нет|
|GetShowToLowStaminaIndication|Возвращает значение индикатора низкой выносливости|нет|float|
|IndicateTooLowAdrenaline|Активирует индикацию слишком низкого уровня адреналина|нет|нет|
|IsThreat|Проверяет, является ли заданный актёр угрозой для игрока|actor: CActor, usePrecalcs: bool|bool|
|StartCSAnim|Запускает анимацию критического состояния|buff: CBaseGameplayEffect|bool|
|AddEffectDefault|Добавляет эффект по умолчанию с возможностью задать продолжительность|effectType: EEffectType, creat: CGameplayEntity, srcName: string, isSignEffect: bool|EEffectInteract|
|SetGuarded|Устанавливает состояние защиты игрока|flag: bool|нет|
|IsGuarded|Проверяет, находится ли игрок в защищённом состоянии|нет|bool|
|GetSelectedItemId|Возвращает ID выбранного предмета|нет|SItemUniqueId|
|ClearSelectedItemId|Сбрасывает выбранный ID предмета|нет||
|IsHoldingItemInLHand|Проверяет, держит ли игрок предмет в левой руке|нет|bool|
|GetCurrentlyUsedItemL|Возвращает текущий используемый предмет в левой руке|нет|W3UsableItem|
|SetPlayerActionToRestore|Устанавливает тип действия игрока для восстановления|actionToRestoreType: EPlayerActionToRestore|нет|
|IsCurrentlyUsingItemL|Проверяет, использует ли игрок предмет в левой руке|нет|bool|
|ProcessUseSelectedItem|Обрабатывает использование выбранного предмета|itemEntity: W3UsableItem, shouldCallOnUsed: bool|нет|
|GetUsableItemTypeById|Возвращает тип используемого предмета по его ID|itemId: SItemUniqueId|EUsableItemType|
|StartWaitForItemSpawnAndProccesTask|Запускает ожидание появления предмета для обработки задачи|нет|нет|
|KillWaitForItemSpawnAndProccesTask|Останавливает ожидание появления предмета для обработки задачи|нет|нет|
|AllowUseSelectedItem|Разрешает использование выбранного предмета|нет|нет|
|CreateInput|Создает обработчик ввода для игрока|нет|нет|
|SetShowToLowStaminaIndication|Устанавливает значение индикатора низкой выносливости|value: float|нет|
|GetShowToLowStaminaIndication|Возвращает значение индикатора низкой выносливости|нет|float|
|IndicateTooLowAdrenaline|Активирует индикацию слишком низкого уровня адреналина|нет|нет|
|IsThreat|Проверяет, является ли заданный актёр угрозой для игрока|actor: CActor, usePrecalcs: bool|bool|
|StartCSAnim|Запускает анимацию критического состояния|buff: CBaseGameplayEffect|bool|
|AddEffectDefault|Добавляет эффект по умолчанию с возможностью задать продолжительность|effectType: EEffectType, creat: CGameplayEntity, srcName: string, isSignEffect: bool|EEffectInteract|
|SetGuarded|Устанавливает состояние защиты игрока|flag: bool|нет|
|IsGuarded|Проверяет, находится ли игрок в защищённом состоянии|нет|bool|
|GetSelectedItemId|Возвращает ID выбранного предмета|нет|SItemUniqueId|
|ClearSelectedItemId|Сбрасывает выбранный ID предмета|нет||
|IsHoldingItemInLHand|Проверяет, держит ли игрок предмет в левой руке|нет|bool|
|GetCurrentlyUsedItemL|Возвращает текущий используемый предмет в левой руке|нет|W3UsableItem|
|SetPlayerActionToRestore|Устанавливает тип действия игрока для восстановления|actionToRestoreType: EPlayerActionToRestore|нет|
|IsCurrentlyUsingItemL|Проверяет, использует ли игрок предмет в левой руке|нет|bool|
|ProcessUseSelectedItem|Обрабатывает использование выбранного предмета|itemEntity: W3UsableItem, shouldCallOnUsed: bool|нет|
|GetUsableItemTypeById|Возвращает тип используемого предмета по его ID|itemId: SItemUniqueId|EUsableItemType|
|StartWaitForItemSpawnAndProccesTask|Запускает ожидание появления предмета для обработки задачи|нет|нет|
|KillWaitForItemSpawnAndProccesTask|Останавливает ожидание появления предмета для обработки задачи|нет|нет|
|AllowUseSelectedItem|Разрешает использование выбранного предмета|нет|нет|
|CreateInput|Создает обработчик ввода для игрока|нет|нет|

