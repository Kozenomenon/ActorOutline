# ActorOutline
Ark Survival Evolved Mod Assets for adding a custom stencil outline to a target actor. Such as a dino.
![ActorOutline](/Images/ActorOutline_Example.png)

## Setup
1. Download the source
2. Place the `ActorOutline` folder in your kit's `/Mods` folder (file explorer, outside the kit)
3. Path in kit to assets listed below should be: `/Game/Mods/ActorOutline`
4. Open `TestMapArea_ActorOutline` 
5. Click PIE button
6. Spawn Dinos & Structures
7. Look at them, see stencil outline on them

## Assets
- **Buff_ActorOutline**
  - *Player buff that enables/disables the stencil.*
  - *Setup to stencil whatever the player is looking at.*
  - *Changed this from what the example did before, left old logic disconnected in BuffClientTick.* 
- **PP_StencilOutlineMaterial**
  - *Base Stencil material with all the visual logic.*
- **PP_StencilOutlineMaterial_MIC**
  - *Material instance referenced by the buff (and your PGD), edit parameters here.*
  
## PIE Things
- **ActorOutline_CCA**
  - *Used so buff applies to player right away in PIE.*
  - *Template used from: [ArkTemplates Open Source](https://github.com/Kozenomenon/ArkTemplates)*
- **PrimalGameData_BP_ActorOutline** 
  - *Test Harness to run the example in PIE.* 
  - *PP MIC in AdditionalBuffPostProcessEffects array.* 
  - *Buff in AdditionalDefaultBuffs array.* 
  - *CCA in Singletons array.* 
- **TestMapArea_ActorOutline** 
  - *Test map to run the example in PIE.* 
 