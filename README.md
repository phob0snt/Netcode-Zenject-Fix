# Netcode-Zenject-Fix
this package will help you to inject dependencies into instantiated network objects. you can test working system by opening test scene.
# IMPORTANT !!!
1. all network objects that you need to spawn with injection ability must be added into NetworkPrefabsInstaller and removed from default network prefabs list
2. spawn network objects with injection ability ONLY USING NetworkManager.SpawnManager.InstantiateAndSpawn() !!! if you just instantiate gameobject and then call spawn injection will not work (idk why =) )
3. required zenject, netcode and multiplayer tools installed
# how to use
1. import unitypackage and drag ZenjectInstallers prefab on scene
2. create zenject project and scene contexts, create networkmanager
3. assign empty default network prefab list to networkmanager
4. add every network prefab that you need in NetworkPrefabsInstaller and assign networkmanager
5. open DependenciesInstaller script and modify it by adding your own bindings
6. now you can [Inject] into instantiated network objects
