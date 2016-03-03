# Unity Utilities : erinylin.lazylib
會秉持懶人精神，朝使用便捷的方向製作。每個專案都會附上範例場景。

## erinylin_fsm.unitypackage
A finite-state machine (FSM), easy to use also can be set by Inspector window.

有限狀態機

![Inspector](https://raw.github.com/erinlin/Unity-Utilities/master/Screenshots/fsm02.jpg)
![ScreenShot](https://raw.github.com/erinlin/Unity-Utilities/master/Screenshots/fsm01.jpg)

## erinylin_sceneloader.unitypackage
Camera-specific component for Scene transition that handle to load the next scene and crossfading between scenes. 

轉場用組件，Camera 專用，處理下個場景載入，順便以交互淡出轉場。只針對掛載的 Camera 畫面作截圖。Canvas 畫面如果需要被印製，需要修改 Rander Mode。
	
	//Add SceneLoader Component in Main Camera.
	using erinylin.lazylib;

	SceneLoader loader = FindObjectOfType<SceneLoader>();
	loader.ToScene = "The Next Scene Name";
	loader.Play();

![SceneLoader](https://raw.github.com/erinlin/Unity-Utilities/master/Screenshots/screenloader01.jpg)