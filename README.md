#Create a script called: PlayerInputErrorFix

#This goes in your script
.
.
.




using UnityEngine;
using UnityEngine.InputSystem;
 
public class PlayerInputErrorFix : MonoBehaviour


{
    
    private PlayerInput Input;
 
    private void Start()
    {
        Input = GetComponent<PlayerInput>();
    }
 
    private void OnDisable()
    {
        Input.actions = null;
    }
}
