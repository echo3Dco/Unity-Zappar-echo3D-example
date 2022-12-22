# Unity-echo3D-Demo-Zappar
Here's a WebAR demo project that integrates echo3D and Zappar SDKs in Unity.

## Setup
* Built with Unity 2020.3.25.  _(Note: The echo3D Unity SDK is supported in 2020.3.25 and higher.)_
* Register for FREE at [echo3D](https://console.echo3D.co/#/auth/register).
* [Add the Unity SDK](https://medium.com/r/?url=https%3A%2F%2Fdocs.echo3d.co%2Funity%2Finstallation). Troubleshoot [here](https://docs.echo3d.com/unity/troubleshooting#im-getting-a-newtonsoft.json.dll-error-in-unity).<br>
* To view a completed demo project that only requires the echo3D API key & entry ID, clone this repo. 

# Video
Watch [here](https://youtu.be/7zCsM5EzvIo).

## Steps
* [Add these models](https://docs.echo3D.co/quickstart/add-a-3d-model) to the echo3D console from the Unity Assets/Models folder:  <br>
   - CowboyHat
* Delete the default camera in the scene. From the Unity toolbar, Zappar > Camera > Front Facing Camera game object from the Zappar menu.
* Add any Zappar Tracking object from the Zappar menu. We used the Face Tracking Target.
* Select the Zappar camera game object and drag the tracking type (in your Hierarchy) into the "Anchor Origin'' property.
* Drag the echo3D script onto an empty parent for your echo3D asset. See CowboyHat in the Hierarchy.  <br>
![Zappar Unity shot](https://user-images.githubusercontent.com/99516371/209229530-a119c8b5-642c-4c81-9949-2ba2ae27e99b.png) <br>
 * [Set the API key](https://docs.echo3d.co/quickstart/access-the-console) and Entry IDs for those same models in the Inspector. <br>
![APIKeyandEntryId](https://user-images.githubusercontent.com/99516371/195749269-f7a43477-b67a-49e8-a212-6abdb9c948fd.png)<br>
![NEWAPIKeyandEntryID](https://user-images.githubusercontent.com/99516371/205407613-b746840f-8e8a-4ec8-b056-a680395dfab4.png)<br>
* [Type your Secret Key](https://docs.echo3d.co/web-console/deliver-pages/security-page#secret-key) as the value for the parameter secKey in the file Packages/co.echo3D.unity/Runtime/Echo3DHologram.cs. _(Note: Secret Key only matters if you have the Security Key enabled). You can turn it off in the Security options in your echo3D console._
![NEWSecKey2](https://user-images.githubusercontent.com/99516371/195749308-b2349a3b-7e43-4d3c-8f09-fbfa9d3cb0be.png)<br>
* (Recommended) To move, resize or edit the assets live in your Scene view, check the boxes for “Editor Preview” and “Ignore Model Transforms”. To enable this, click Echo3D > Load Editor Holograms in your Unity toolbar. <br>
![EditorPreviewAndIgnoreModelTransforms](https://user-images.githubusercontent.com/99516371/195749348-dc0b06ad-efa6-4dbd-962f-0119b5c33ea0.png)<br>
![LoadHolograms](https://user-images.githubusercontent.com/99516371/195749354-b2295183-f877-444a-af22-ed87ffb17705.png) <br>
* Change Build Settings to WebGL.
* Go to Build Settings > Player > Resolution and Presentation and select the Zappar player (Zappar for 2020+, or Zappar 2019 for anything older).

## Run
Build for WebGL, view WebAR experience through desktop browser. Desktop camera access is required.

## Learn More
Refer to our [documentation](https://docs.echo3D.co/unity/) to learn more about how to use Unity and echo3D.

## Troubleshooting
Visit our troubleshooting guide [here](https://docs.echo3d.co/unity/troubleshooting#im-getting-a-newtonsoft.json.dll-error-in-unity).

## Support
Feel free to reach out at [support@echo3D.co](mailto:support@echo3D.co) or join our [support channel on Slack](https://go.echo3D.co/join). 
