```
enum EActorImmortalityMode
{
	AIM_None,
	AIM_Immortal,				
	AIM_Invulnerable,			
	AIM_Unconscious				
}
```
```
enum EActorImmortalityChanel
{
	
	AIC_Default = 1,
	AIC_Combat = 2,
	AIC_Scene = 4,
	AIC_Mutation11 = 8,
	AIC_Fistfight = 16,
	AIC_SyncedAnim = 32,
	AIC_WhiteRaffardsPotion = 64,
	AIC_IsAttackableByPlayer = 128
	
}
```
```
enum EActorImmortalityMode
{
	AIM_None,
	AIM_Immortal,				
	AIM_Invulnerable,			
	AIM_Unconscious				
}
```
```
enum EStaminaActionType
{
	ESAT_Undefined,
	ESAT_LightAttack,
	ESAT_HeavyAttack,
	ESAT_SuperHeavyAttack,
	ESAT_Parry,
	ESAT_Counterattack,
	ESAT_Dodge,
	ESAT_Evade,
	ESAT_Swimming,
	ESAT_Sprint,
	ESAT_Jump,
	ESAT_UsableItem,
	ESAT_Ability,
	ESAT_FixedValue,
	ESAT_Roll,
	ESAT_LightSpecial,
	ESAT_HeavySpecial,
}
```
```
enum ECharacterPowerStats
{
	CPS_AttackPower,
	CPS_SpellPower,
	CPS_Undefined
}
```
```
function StatEnumToName(s : EBaseCharacterStats) : name
{
	switch(s)
	{
		case BCS_Vitality : 		return 'vitality';
		case BCS_Essence : 			return 'essence';
		case BCS_Stamina : 			return 'stamina';
		case BCS_Toxicity : 		return 'toxicity';
		case BCS_Focus : 			return 'focus';
		case BCS_Morale : 			return 'morale';
		case BCS_Air 		: 		return 'air';
		case BCS_Panic	:			return 'panic';
		case BCS_PanicStatic :		return 'panicStatic';
		case BCS_SwimmingStamina :	return 'swimmingStamina';
		default:					return '';
	}
}
```
```
function StatNameToEnum(n : name) : EBaseCharacterStats
{
	switch(n)
	{
		case 'vitality' : 			return BCS_Vitality;
		case 'essence' : 			return BCS_Essence;
		case 'stamina' : 			return BCS_Stamina;
		case 'toxicity' : 			return BCS_Toxicity;
		case 'focus' : 				return BCS_Focus;
		case 'morale' : 			return BCS_Morale;
		case 'air' : 				return BCS_Air;
		case 'panic' : 				return BCS_Panic;
		case 'panicStatic' :		return BCS_PanicStatic;
		case 'swimmingStamina' :	return BCS_SwimmingStamina;
		default:					return BCS_Undefined;
	}
}
```
```
enum ECharacterRegenStats
{
	CRS_Undefined,
	CRS_Vitality,
	CRS_Essence,
	CRS_Morale,
	CRS_UNUSED,
	CRS_Stamina,
	CRS_Air,
	CRS_Panic,
	CRS_SwimmingStamina,
}
```
```
function ResistStatEnumToName(s : ECharacterDefenseStats, isPointResistance : bool) : name
{
	if(isPointResistance)
	{
		switch(s)
		{
			case CDS_PhysicalRes :				return 'physical_resistance';
			case CDS_PoisonRes :				return 'poison_resistance';
			case CDS_FireRes :					return 'fire_resistance';
			case CDS_FrostRes :					return 'frost_resistance';
			case CDS_ShockRes :					return 'shock_resistance';
			case CDS_ForceRes :					return 'force_resistance';
			case CDS_SlashingRes :	 			return 'slashing_resistance';
			case CDS_PiercingRes :				return 'piercing_resistance';
			case CDS_BludgeoningRes:			return 'bludgeoning_resistance';
			case CDS_RendingRes : 				return 'rending_resistance';
			case CDS_ElementalRes : 			return 'elemental_resistance';
			case CDS_DoTBurningDamageRes : 		return 'burning_DoT_damage_resistance';
			case CDS_DoTPoisonDamageRes :		return 'poison_DoT_damage_resistance';
			case CDS_DoTBleedingDamageRes : 	return 'bleeding_DoT_damage_resistance';
			default :							return '';
		}
	}
	else
	{
		switch(s)
		{
			case CDS_PhysicalRes :				return 'physical_resistance_perc';
			case CDS_BleedingRes : 				return 'bleeding_resistance_perc';
			case CDS_PoisonRes :				return 'poison_resistance_perc';
			case CDS_FireRes :					return 'fire_resistance_perc';
			case CDS_FrostRes :					return 'frost_resistance_perc';
			case CDS_ShockRes :					return 'shock_resistance_perc';
			case CDS_ForceRes :					return 'force_resistance_perc';
			case CDS_WillRes :					return 'will_resistance_perc';
			case CDS_BurningRes : 				return 'burning_resistance_perc';
			case CDS_SlashingRes :	 			return 'slashing_resistance_perc';
			case CDS_PiercingRes :				return 'piercing_resistance_perc';
			case CDS_BludgeoningRes:			return 'bludgeoning_resistance_perc';
			case CDS_RendingRes : 				return 'rending_resistance_perc';
			case CDS_ElementalRes :				return 'elemental_resistance_perc';
			case CDS_DoTBurningDamageRes : 		return 'burning_DoT_damage_resistance_perc';
			case CDS_DoTPoisonDamageRes :		return 'poison_DoT_damage_resistance_perc';
			case CDS_DoTBleedingDamageRes : 	return 'bleeding_DoT_damage_resistance_perc';
			default :							return '';
		}
	}
}

```
