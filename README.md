# inventoryInUnity
Inventory assets and manual to set-up fast.

----------
  MANUAL 
----------

1. Create a new script called "Item" and paste the script from the github.

2. Add an Image to the Canvas.

3. Replace the image by your borderHealthBar sprite.

4. Create a new empty called "HealthBar" in the Canvas

5. Re-size the HealthBar as the borderHealthBar sprite in the scene.

6. Create border a child of HealthBar.

7. Create an image named "Fill" in the health bar : Right click HealthBar --) UI/Image.

8. Place "Fill" over "Border" in the hierarchy (inspector).

9. Re-size "Fill" so it matches correctly with "Border".
    - If you're making a rectangle or squared-shaped healthBar, you can simply do an auto stretch in [Rect Transform] in the inspector.
    - If you're making a special-shaped healthBar, resize manually.

10. Add to HealthBar a "Slider" component.

11. Uncheck "Interactible".
---------------------------
Additional intel :
Interactible makes the healthBar clickable : for example, if we click on the middle of the healthBar, the "Fill" will stretch itself to the middle. This is why we're unchecking it.
---------------------------

12. Set "Transition" and "Navigation" to "None".

13. Click & Drag "Fill" in the "Fill Rect" fill.

14. Set Max Value to 100. This is your HP max number.

15. Set "Value" to 100.

16. You can now proceed to adding more visual content around your healthBar (like a heart to the left).
Don't forget the "Set Native Size" option if your sprites are weirdly shaped.
You may anchor your new stuff.

17. You may now re-size your health bar correctly (I mean making it visible and well-placed on your game output).

18. Add a new script to HealthBar named as it ("HealthBar").

19. Copy & Paste the contents of "HealthBar" from the github to your Unity script.

20. Add a new (component) script named "PlayerHealth" to your playable character.

21. Copy & Paste the contents of "PlayerHealth" from the github to your Unity script.

22. Add the object reference "HealthBar" in the fill in "PlayerHealth" script.

22. Add to the HealthBar the component reference "Slider" in the fill in "HealthBar" script.

To create a scriptable object when the "Item" script has been added and loaded, go to Assets/Inventory/Item.




x. Make a script called "Inventory"