# Open-Vtube

### Feasibility study for achieving Live2D-like result with only open source resources.<br>僅使用開源資源製作出類似Live2D效果的可行性研究。

1. <b>Model building 建模</b>  
    <b>[Blender](https://www.blender.org/):</b> Blender可以用Shape key改變Mesh的形狀，理論上可以做到跟Live2D一樣的效果，甚至可以做到Live2D做不到的立體效果。


2. <b>Rendering 模型渲染</b>  
    <b>[Blender](https://www.blender.org/):</b> 直接在Blender的viewport上render，如果只用圖片的話可以直接viewport shading，如果需要更加複雜的shader的話可以使用Eevee renderer。把viewport的背景換成綠色就可以色鍵去背。
    
    Blender的物理系統使用timeline，無法在viewport中無限播放，但可以用python script每frame更新物件。


3. <b>Streaming 直播</b>  
    <b>[OBS](https://obsproject.com/):</b> 長久以來直播主使用的OBS就是開源軟件，不需要尋找替代品。

4. <b>Face mesh 面容定位</b>  
    <b>[Mediapipe](https://github.com/google/mediapipe):</b> Mediapipe是Google的開源人工智能工具，可以用作面容定位。其他現存的Blender面容定位方案例如OpenPose，Ai Face都不是開源方案。


5. <b>Hand detection 手勢辨識</b>  
    <b>[Mediapipe](https://github.com/google/mediapipe):</b> Mediapipe亦可以用作手勢辨識。


6. <b>Emotion recognition 表情辨識</b>  
    <b>[Emotion-detection](https://github.com/atulapra/Emotion-detection):</b> 這個看來可以用。
