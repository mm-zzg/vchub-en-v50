# findFire

**Description**: Query the first fire special effect that meets the criteria in the scene

Query fire:

```typescript
const view = await System.UI.findControl('3DViewer1')// Obtain a 3D viewer control named "3DViewer1" in the page
const scene = await view.getScene();
const mash = await scene.findFire('fire')//Query for special effects where the name includes fire
console.log(mash)//Output all queried results
```
 
**Example:**

Write the above code on the button, click the button, and you can query the first fire special effect in the scene whose name includes fire

![img](https://docs.wagoscada.cn/wiki/api/wiki/external-editor/QHXVK91b/4BsBCyyr/resources/GOsS_L5aIyAKwyjE48ZMzs9LLFe-McT7pMbHLtp283Q.gif)

The queried model can use all its methods and properties:

# findFire

**Description**: Query the first fire special effect that meets the criteria in the scene

Query fire:

```typescript
const view = await System.UI.findControl('3DViewer1')// Obtain a 3D viewer control named "3DViewer1" in the page
const scene = await view.getScene();
const mash = await scene.findFire('fire')//Query for special effects where the name includes fire
console.log(mash)//Output all queried results
```
 
**Example:**

Write the above code on the button, click the button, and you can query the first fire special effect in the scene whose name includes fire

![1](../../../assets/images/3d_lowcode_SOperation_findfire1.gif)

The queried model can use all its methods and properties:

![alt text](3d_lowcode_SOperation_findfire2.png)


