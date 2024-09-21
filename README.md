# glTFast with script exporting
## What's different?
This version of glTFast based on the 6.8.0 release. The only difference is SerializeMonoBehaviours method in class GameObjectExport. It is added to serialize all MonoBehaviours and their serialized properties data to "extras" token of each node.
Example gltf output: 
{"name":"Doc house","children":[80],"translation":[-9.05,8.418393,-45.84],"rotation":[-9.66888E-08,0.09672506,1.15608669E-08,0.995311141],"scale":[0.563429832,0.945775747,1.39120018],"extras":[
  {
    "TypeName": "InteractableObject",
    "OnInteract": "UnityEngine.Events.UnityEvent`1[CharacterController] UnityEngine.Events.UnityEvent`1[[CharacterController, Assembly-CSharp, Version=0.0.0.0, Culture=neutral, PublicKeyToken=null]]"
  },
  {
    "TypeName": "DialogueStarter",
    "dialogue": null,
    "npc": null,
    "player": null
  }
]}
For additional information please refer to original repo: https://github.com/atteneder/glTFast
## License

Copyright 2023 Unity Technologies and the Unity glTFast authors

Licensed under the Apache License, Version 2.0 (the "License");
you may not use files in this repository except in compliance with the License.
You may obtain a copy of the License at

   <http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

## Trademarks

*Unity&reg;* is a registered trademark of [Unity Technologies][unity].

*Khronos&reg;* is a registered trademark and [glTF&trade;][gltf] is a trademark of [The Khronos Group Inc][khronos].

[gltf-spec]: https://www.khronos.org/registry/glTF/specs/2.0/glTF-2.0.html
[gltf]: https://www.khronos.org/gltf
[gltfasset_component]: ./Documentation~/Images/gltfasset_component.png  "Inspector showing a GltfAsset component added to a GameObject"
[import-gif]: ./Documentation~/Images/import.gif  "Video showing glTF files being copied into the Assets folder and imported"
[khronos]: https://www.khronos.org
[unity]: https://unity.com
[UnityGltfast]: https://docs.unity3d.com/Packages/com.unity.cloud.gltfast@latest/
[workflows]: ./Documentation~/index.md#workflows
