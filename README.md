# LiberatingMarsCLI
**We don't want to be forced into which Slicer we use. Let's change that.**

### Usage:
LiberatingMarsCLI(.exe) <Mandatory Arguments> [Optional Arguments]
  
  Mandatory Arguments:
  
    Path to ChiTuBox 1.9.0 executable
  
    Path to legacy CTB file
  
  Optional Arguments:
  
    Slow Lift Height    : The height of the initial slow lift. This must be a lower value than the total lift height. 
                          The build platform will do a slow lift to this position, and then a fast lift the rest of the way to the total lift height 
                          In Formware the speed in this section will be either "Z Lift Speed" or "Z Bottom Speed"
  
    Slow Retract Height : The height of the final slow retract. This must be lower than the total lift height.
                          The build platform will do a fast retract from the top of the total lift height to this height above the next layer and then a slow
                          retract the rest of the way.
                          In Formware the speed in this section will be either "Z Lift Speed" or "Z Bottom Speed"
  
    Pause Before Lift   : The time in seconds to pause after exposure and before lift
  
    Pause After Lift    : The time in seconds to pause after lift and before retract
  
    Pause After Retact  : The time in seconds to pause after retract and before exposure

In Formware, the fast lift and fast retract speeds will be "Z Retract Speed"
  
### Output:
[file name].ctb (The original file is overwritten)

