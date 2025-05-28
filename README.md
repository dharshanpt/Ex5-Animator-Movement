# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : DHARSHAN PT
### REG NO : 212223230046

## PlayerController:


```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent <Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputX", InputX);
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputY", InputY);
    }
}


```
## Output :
![5 1](https://github.com/user-attachments/assets/b6a83409-7182-4884-b24e-ebe4cb9afccf)

![5 2](https://github.com/user-attachments/assets/84e396c6-5116-40c1-8842-2f4cfd0dc194)
![5 3](https://github.com/user-attachments/assets/6207a343-96a3-49f6-99d6-39b3f73ea31d)


## Result :

Thus, An animator movement for a player using unity is developed successfully.
