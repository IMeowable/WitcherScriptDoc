Я думаю, что эти методы можно вызвать статически от thePlayer.Method().

|Функция|Описание|
| :-: | :-: |
|GetInputHandler() : CPlayerInput|Возвращает обработчик ввода для игрока.|
|IsInCombatState() : bool|Проверяет, находится ли игрок в состоянии боя.|
|DisableCombatState()|Отключает состояние боя, переводя игрока в режим исследования.|
|GetHowLongSprintButtonWasPressed() : float|Возвращает длительность нажатия кнопки спринта.|
|IsSprintActionPressed() : bool|Проверяет, нажата ли кнопка спринта.|
|GetIsSprintToggled() : bool|Возвращает состояние переключения спринта.|
|SetWalkToggle(flag : bool)|Устанавливает состояние переключения ходьбы.|
|GetIsWalkToggled() : bool|Возвращает состояние переключения ходьбы.|
|GetIsRunning() : bool|Возвращает состояние бега игрока.|
|SetIsRunning(flag : bool)|Устанавливает состояние бега игрока.|
|GetIsWalking() : bool|Возвращает состояние ходьбы игрока.|
|SetIsWalking(walking : bool)|Устанавливает состояние ходьбы игрока.|
|SetIsMovable(flag : bool)|Устанавливает, может ли игрок двигаться.|
|SetManualControl(movement : bool, camera : bool)|Устанавливает ручное управление движением и камерой, если отключено движение, поднимает событие "Idle".|
|IsInCombatAction\_SpecialAttack() : bool|Проверяет, находится ли игрок в специальной боевой атаке.|
|SetBIsInCombatAction(flag : bool)|Устанавливает состояние боевого действия, изменяя соответствующую переменную поведения.|
|SetVehicleCachedSign(sign : ESignType)|Устанавливает запомненный знак для транспортного средства.|
|GetVehicleCachedSign() : ESignType|Возвращает запомненный знак для транспортного средства.|
|GetMoney() : int|Возвращает количество денег у игрока.|
|AddMoney(amount : int)|Добавляет указанное количество денег игроку.|
|GetEquippedSign() : ESignType|Возвращает текущий экипированный знак.|
|GetCurrentlyCastSign() : ESignType|Возвращает знак, который в данный момент кастуется.|
|IsCastingSign() : bool|Проверяет, кастует ли игрок знак.|
|IsCurrentSignChanneled() : bool|Проверяет, является ли текущий знак канализированным.|

