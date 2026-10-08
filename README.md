# Potion-Generator
Procedural potion generator that allows you to change the shape and scale off different aspects of the bottle. 
Made in Blender 5.2.1

**How to use:**
1. Duplicate the potion object and PotionGen_LOD0 below it
2. Edit the parameters in the modifiers tab to get desired bottle shape
   - **Bottle type:** changes the base shape
   - **Base scale:** changes the scale of body of the bottle
   - **Stopper type:** switches between A (normal cork) and B (sphere cork)
   - **Stopper radius:** radius if the cork
   - **Bottleneck radius:** radius if the stem of the bottle
   - **Bottleneck length:** changes how long the bottle stem is
   - **Level of Detail:** changes resolution of bottle, 0 is highest resolution and 2 is lowest
3. Once you have the desired bottle you can create the LODs
   - Duplicate the PotionGen_LOD0 that you modified twice, make sure they appear under the same parent object
   - Change the end of one to _LOD1 and in the modifier set level of detail to 1
   - Change the end of the other to _LOD2 and in the modifier set level of detail to 2
   - Select the parent object and all three PotionGens underneath
   - Go to File --> Export --> FBX
   - Check the boxes that say
          - **Selected Objects**
          - **Custom Properties**
          - **Apply Transform**
