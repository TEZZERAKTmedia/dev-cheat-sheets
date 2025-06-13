# 🎮 Unity C# (AR) Cheat Sheet

## 🛠 Script Example
```csharp
public class DoorSpawner : MonoBehaviour {
    public GameObject prefab;

    void Spawn() {
        Instantiate(prefab, transform.position, Quaternion.identity);
    }
}
```

## 🔁 Input & Raycasting
```csharp
if (Input.touchCount > 0) {
    Touch touch = Input.GetTouch(0);
    if (raycastManager.Raycast(touch.position, hits)) {
        Pose hitPose = hits[0].pose;
    }
}
```

## 🪄 Prefab Management
- Use `Instantiate`
- Use `SetActive(false)` to toggle