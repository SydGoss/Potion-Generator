# Potion-Generator
Procedural potion generator that allows you to change the shape and scale off different aspects of the bottle. 
Made in Blender 5.2.1

**How to use:**
1. Duplicate the potion object and PotionGen_LOD0 below it
2. Edit the parameters in the modifiers tab to get desired bottle shape
3. Once you have the desired bottle you can create the LODs
   - Duplicate the PotionGen_LOD0 that you modified twice, make sure they appear under the same parent object
   - Change the end of one to _LOD1 and in the modifier set level of detail to 1
   - Change the end of the other to _LOD2 and in the modifier set level of detail to 2
   <img width="416" height="529" alt="Screenshot 2026-10-08 at 12 14 51 AM" src="https://github.com/user-attachments/assets/67852c1f-8363-4057-b1c4-69411772008e" />


   - Select the parent object and all three PotionGens underneath
   - Go to File --> Export --> FBX
   - Check the boxes that say
          - **Selected Objects**
          - **Custom Properties**
          - **Apply Transform**

4. Import the FBX to Unreal using the import button or by dragging it from your files into the content browser
5. In the import settings pop-up uncheck **recompute normals** and then click import
<img width="628" height="110" alt="Screenshot 2026-10-08 at 1 47 13 AM" src="https://github.com/user-attachments/assets/2992af08-bd48-4ddc-a8f5-1caf72c37b21" />


