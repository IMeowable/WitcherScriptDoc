
#types and enums at W3PlayerWitcher class

enum ESignType
{
	ST_Aard,
	ST_Yrden,
	ST_Igni,
	ST_Quen,
	ST_Axii,
	ST_None
}

CActor базовый класс для классов игроков.

enum EEffectType
{
	EET_Undefined,		

	
	EET_AutoVitalityRegen,
	EET_AutoStaminaRegen,
	EET_AutoEssenceRegen,
	EET_AutoMoraleRegen,
		
	
	EET_Confusion,
	EET_HeavyKnockdown,
	EET_Hypnotized,
	EET_Immobilized,
	EET_Knockdown,	
	EET_KnockdownTypeApplicator,
	EET_Frozen,
	EET_Paralyzed,
	EET_Stagger,
	EET_Blindness,
	EET_PoisonCritical,
				
	
	EET_Bleeding,
	EET_BleedingTracking,
	EET_Burning,
	EET_Poison,
	EET_DoTHPRegenReduce,
		
	
	EET_Toxicity,
		
	
	EET_BlackBlood,
	EET_Blizzard,
	EET_Cat,
	EET_FullMoon,
	EET_GoldenOriole,
	EET_MariborForest,
	EET_PetriPhiltre,
	EET_Swallow,
	EET_TawnyOwl,

	EET_Thunderbolt,
EET_Unused1,
	EET_WhiteHoney,
	EET_WhiteRaffardDecoction,
	EET_KillerWhale,
	
	
	EET_AxiiGuardMe,
	EET_IgnorePain,
	
	
	EET_StaggerAura,
	EET_OverEncumbered,
	EET_Edible,	
	EET_LowHealth,
	EET_Slowdown,
	EET_Fact,
	EET_WellFed,
	EET_SlowdownFrost,
	
	
	EET_LongStagger,				
	EET_WellHydrated,
	EET_BattleTrance,				
	EET_YrdenHealthDrain,
	EET_AdrenalineDrain,
	EET_WeatherBonus,
	EET_Swarm,						
	EET_Pull,						
	EET_AbilityOnLowHealth,			
	EET_Oil,
	EET_CounterStrikeHit,	
	EET_Drowning,
	EET_Snowstorm,	
	EET_AutoAirRegen,
	
	
	EET_ShrineAard,
	EET_ShrineAxii,
	EET_ShrineIgni,
	EET_ShrineQuen,
	EET_ShrineYrden,
	
	
	EET_Ragdoll,	
	EET_AutoPanicRegen,	
	EET_VitalityDrain,
	EET_DoppelgangerEssenceRegen,	
	EET_FireAura,	
	EET_BoostedEssenceRegen,
	EET_AirDrain,
	EET_SilverDust,

	
	EET_Mutagen01,
	EET_Mutagen02,
	EET_Mutagen03,
	EET_Mutagen04,
	EET_Mutagen05,
	EET_Mutagen06,
	EET_Mutagen07,
	EET_Mutagen08,
	EET_Mutagen09,
	EET_Mutagen10,
	EET_Mutagen11,
	EET_Mutagen12,
	EET_Mutagen13,
	EET_Mutagen14,
	EET_Mutagen15,
	EET_Mutagen16,
	EET_Mutagen17,
	EET_Mutagen18,
	EET_Mutagen19,
	EET_Mutagen20,
	EET_Mutagen21,
	EET_Mutagen22,
	EET_Mutagen23,
	EET_Mutagen24,
	EET_Mutagen25,
	EET_Mutagen26,
	EET_Mutagen27,
	EET_Mutagen28,
	
	
	EET_AirDrainDive,
	EET_BoostedStaminaRegen,
	EET_WitchHypnotized,
	EET_AirBoost,
	EET_StaminaDrainSwimming,
	EET_AutoSwimmingStaminaRegen,
	EET_Drunkenness,
	EET_WraithBlindness,
	EET_Choking,
	EET_StaminaDrain,
	EET_EnhancedArmor,
	EET_EnhancedWeapon,
	EET_SnowstormQ403,
	EET_SlowdownAxii,
	EET_PheromoneNekker,
	EET_PheromoneDrowner,
	EET_PheromoneBear,
	EET_Tornado,
	EET_WolfHour,
	EET_WeakeningAura,
	EET_Weaken,
	
	EET_Tangled,					
	EET_Runeword8,
	EET_LynxSetBonus,
	EET_GryphonSetBonus,
	EET_GryphonSetBonusYrden,
	EET_POIGorA10,
	EET_Mutation7Buff,
	EET_Mutation7Debuff,
	EET_Mutation10,
	EET_Perk21InternalCooldown,
	EET_Mutation11Buff,
	EET_Mutation11Debuff,	
	EET_Acid,						
	EET_WellRested,
	EET_HorseStableBuff,
	EET_BookshelfBuff,
	EET_PolishedGenitals,
	EET_Mutation12Cat,
	EET_Mutation11Immortal,
	EET_Aerondight,
	EET_Trap,
	EET_Mutation3,
	EET_Mutation4,
	EET_Mutation5,
	EET_ToxicityVenom,
	EET_BasicQuen,
	
	
	EET_ReinaldPhiltre,
	
	
	EET_Bleeding1,
	EET_Bleeding2,
	EET_Bleeding3,
	
	
	
	
EET_EffectTypesSize,
EET_ForceEnumTo16Bit = 10000
}

enum ESkill
{
	S_SUndefined,
	
	S_Sword_1,				
	S_Sword_2,				
	S_Sword_3,				
	S_Sword_4,				
	S_Sword_5,				
	
	S_Magic_1,				
	S_Magic_2,				
	S_Magic_3,				
	S_Magic_4,				
	S_Magic_5,				
	
	S_Alchemy_1,			
	S_Alchemy_2,			
	S_Alchemy_3,			
	S_Alchemy_4,			
	S_Alchemy_5,			
	
	
	S_Sword_s01,			
	S_Sword_s02,			
	S_Sword_s03,			
	S_Sword_s04,			
	S_Sword_s05,			
	S_Sword_s06,			
	S_Sword_s07,			
	S_Sword_s08,			
	S_Sword_s09,			
	S_Sword_s10,			
	S_Sword_s11,			
	S_Sword_s12,			
	S_Sword_s13,			
S_UNUSED1,
	S_Sword_s15,			
	S_Sword_s16,			
	S_Sword_s17,			
	S_Sword_s18,			
	S_Sword_s19,			
	S_Sword_s20,			
	S_Sword_s21,			
	
	
	S_Magic_s01,			
	S_Magic_s02,			
	S_Magic_s03,			
	S_Magic_s04,			
	S_Magic_s05,			
	S_Magic_s06,			
	S_Magic_s07,			
	S_Magic_s08,			
	S_Magic_s09,			
	S_Magic_s10,			
	S_Magic_s11,			
	S_Magic_s12,			
	S_Magic_s13,			
	S_Magic_s14,			
	S_Magic_s15,			
	S_Magic_s16,			
	S_Magic_s17,			
	S_Magic_s18,			
	S_Magic_s19,			
	S_Magic_s20,			
S_UNUSED2,
	
	
	S_Alchemy_s01,			
	S_Alchemy_s02,			
	S_Alchemy_s03,			
	S_Alchemy_s04,			
	S_Alchemy_s05,			
	S_Alchemy_s06,			
	S_Alchemy_s07,			
	S_Alchemy_s08,			
	S_Alchemy_s09,			
	S_Alchemy_s10,			
	S_Alchemy_s11,			
	S_Alchemy_s12,			
	S_Alchemy_s13,			
	S_Alchemy_s14,			
	S_Alchemy_s15,			
	S_Alchemy_s16,			
	S_Alchemy_s17,			
	S_Alchemy_s18,			
	S_Alchemy_s19,			
	S_Alchemy_s20,			
	S_Skill_MAX,

	S_Perk_MIN,
	S_Perk_01,				
	S_Perk_02,				
	S_Perk_03,				
	S_Perk_04,				
	S_Perk_05,				
	S_Perk_06,				
	S_Perk_07,				
	S_Perk_08,				
	S_Perk_09,				
	S_Perk_10,				
	S_Perk_11,				
	S_Perk_12,				
	
	
	S_Perk_13,				
	S_Perk_14,				
	S_Perk_15,				
	S_Perk_16,				
	S_Perk_17,				
	S_Perk_18,				
	S_Perk_19,				
	S_Perk_20,				
	S_Perk_21,				
	S_Perk_22,				
	S_Perk_MAX
}

enum ESkillPath
{
	ESP_NotSet,
	ESP_Sword,
	ESP_Signs,
	ESP_Alchemy,
	ESP_Perks
}

enum ESpendablePointType
{
	ESkillPoint,
	EExperiencePoint
}

struct SItemUniqueId { }



