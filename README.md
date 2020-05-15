# ActorOutline
Ark Survival Evolved Mod Assets for adding a custom stencil outline to a target actor. Such as a dino.

## Assets
- **Buff_ActorOutline**
  - *Player buff that enables/disables the stencil.*
- **PP_StencilOutlineMaterial**
  - *Stencil material with all of the graph logic.*
- **PP_StencilOutlineMaterial_MIC**
  - *Material instance referenced by the buff (and your PGD), edit parameters here.*
 
## Setup
1. Download this source
2. [Unblock](https://lmgtfy.com/?q=unblock+windows+file) the .asset files in Windows File Explorer
3. Place assets in your mod folder *(best if ADK is closed when you do this)*
4. Open your mod PGD and add 'PP_StencilOutlineMaterial_MIC' to the 'Additional Buff Post Process Effects' array 
5. Implement the means within your mod to 'Static Add Buff' on the Player referencing the 'Buff_ActorOutline' 
   - *The desired stencil target needs to be set as 'Damage Causer' when you do this.*
6. Deactivate the buff to remove the stencil from display. 
