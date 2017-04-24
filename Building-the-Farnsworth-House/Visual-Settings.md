### Visual Settings
Moving your conceptual model to Revit for documentation is only half of the deliverables that come from FormIt. The other half are beautiful graphics that help to tell a story to a client, or team member. We'll cover ways to set up your **camera scenes**, your **graphic visual styles**, and **export your images** at high resolution.

If you did not complete the last section, download and open the **farnsworth10.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

#### Scenes

1. Open the **Scenes** palette

    ![](./images/ScenesIcon.png)

2. **Double click** the only saved Scene - the camera animates to take you to that stored viewpoint 

3. The visual styles, shadow settings, and layer states update to what was stored when that scene was set up

2. In the [**Scenes Palette**](../formit-introduction/tool-bars.md) click the **"+"** icon to add a new scene

3. In the **Scene Properties** - lower in the palette - rename the new scene and **Aerial**. The checkboxes determine whether changes to these settings affect the scene

    ![](./images/777d3348-1472-4afb-a617-54bffb9b947f.png)

4. Navigate the camera to an aerial view. Turn on the **trees** layer and turn off the **plan image** layer

    ![](./images/a3529158-1a4a-4fac-a8ee-6f60247bce4d.png)

5. **Single click** on the **Aerial** scene and then click the **update** icon. This will reset the scene to the current camera viewpoint and properties

    ![](./images/a6828bff-7d6e-4cc9-b00c-1db0de96d0b1.png) 

7. Press the **Play** icon to animate the camera through the saved scenes

    ![](./images/7badfc11-b64f-45d4-b0d3-0433ce8c5b79.png)
    
1. Click the **Stop** icon to end the animation

#### Visual Styles

2. **Double click** the original **Scene** to navigate to it. Turn on the **trees** layer and turn off the **plan image** layer

2. Select the [**Visual Styles Palette**](../formit-introduction/tool-bars.md). There are four tabs at the top for different effects: **Surfaces**, **Edges**, **Environment**, and **Model Diagnostics**

    ![](./images/aa340156-b0de-4132-8b24-98fe2533dbfe.png)

4. Turn **Monotone Surfaces (DM)** on. This makes an abstract black and white image without any materials. To turn Monotone off just type DM again

    ![](./images/74f592a0-e7b3-4168-a6e9-2d1f69453f54.png)

5. Turn on **Ambient Shadows (DA)**, and from the Edge tab, adjust the sliders to lighten the contrast of the edges and silhouettes to **30%**. Also turn on the **Extend Edges (DX)**

    ![](./images/74f592a0-e7b3-4168-a6e9-2d1f69453f54_2.png)
    
6. You can update the scene to record the changes, or click the **"+"** icon to save a new scene with the current settings

#### Section Planes
When working with Scenes, Graphics, Layers, and other settings you can also introduce multiple **Section Planes** to see inside of your model

2. Click the Section icon from the **main toolbar**

    ![](./images/sectionIcon.png)
    
2. Hover your mouse over one of the glass faces - the arrow indicators show that the section will cut **into** the building

    ![](./images/SectionTemp.png)

2. **Click** to place the **Section plane**. The plane scales to the size of your model, and stays selected (hence the blue color) 

3. Click the plane start the **move** tool and push the plane **inward**. Click again to **place** the plane down. Once you're happy with the location of the Section Plane, **click Esc** to clear the selection

    ![](./images/Section_1.png)
    
4. Go to the **Layers** tab. Two new layers have been generated - **Section Indicators** and **Section Cut 1**. Toggle **Section Cut 1** off and back on. This controls the cut effect. Now toggle the **Section Indicator** layer off, this hides the plane, and the arrow indicators
    
4. Go to the **Visual Styles** tab. On the **Surfaces** panel, turn on the Poche color - it defaults to Black. This effect will color the inside faces of the section cut with a specified color

    ![](./images/Section_2.png)

5. You can add up to **6 section cuts** to your model. You can experiment by navigating to the **Aerial View** scene and placing a section plane that removes the roof

6. Make sure to return to the Scenes tab and update your scenes, so that your Section graphics are stored 

#### Export Image

1. Click **File &gt; Export (Ctrl + E)**

2. Choose **As Image** from the bottom of the list

3. Choose the resolution from the Preset drop down list. Note that if you have any element selected in the canvas, the selection color will be exported too

    ![](./images/03b98705-6f53-4856-aea7-a48a906b981f.png)
    
If you want to the file for this completed section, download and open the **farnsworth11.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).