1. Only one camera can have the SteamVR_Camera component, or Unity will crash.

2. The correct configuration is the original Eye cam used for left eye, and a
second Eye cam for right eye parented above it, to the root of the prefab.
Remove the SteamVR_Camera component from the right Eye.

3. Then parent each of your rendertexture cameras beneath the Eye cams.

4. The rendertexture cams need to have their projection matrix corrected; see:  
https://steamcommunity.com/app/358720/discussions/0/405694031550581171/#c4056940
31552884526
