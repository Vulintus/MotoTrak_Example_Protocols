# MotoTrak Isometric Pull Shaping/Training Example Protocol for Rats

*Updated 2024-08-15*

<ins>**NOTE:**</ins> This protocol is meant to serve as one example of how rats can be trained on the isometric pull task with MotoTrak, but it is by no means the *only* way to train rats. Different labs may use different task parameters, different training steps, different session lengths and frequencies, and different timelines based on their particular models.

## Stage and Implementation Files:

Stage definition and implementation files, used with the MotoTrak Version 2.0 behavioral program, corresponding to the training/testing stages described in this protocol are hosted and maintained in a public [Github repository](https://github.com/Vulintus/MotoTrak_Example_Protocols). A zip file containing the stage definition and implementation files for this example protocol can also be downloaded from this link:

[Rat Isometric Pull Example Files - Rat (zip)](https://github.com/Vulintus/MotoTrak_Example_Protocols/raw/main/Isometric%20Pull%20-%20Rat/MotoTrak_Isometric_Pull_Protocol_Rat.zip)

After you unzip the files, you’ll see a folder named “Stages” which contains stage definition files, ending in the extension *.MOTORSTAGE, and you’ll see a Python file called “PythonPullStageImplementationRat.py”. We’re going to put the two file types in different places.

First, copy/cut all of the *.MOTORSTAGE files and paste them into MotoTrak’s “Stages” folder, which you can get to from the main menu by clicking *Open configuration folder*.



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

<img width="516" height="392" alt="mototrak_v2p0_main_menu_open_configuration_folder_selected" src="https://github.com/user-attachments/assets/af638671-58c7-4b00-aa6d-c58c4122bb9c" />

Next, copy/cut the “PythonPullStageImplementationRat.py” Python file and past it into the following folder (you will likely need administrator permissions on the computer you’re using):

C:\Program Files (x86)\Vulintus\MotoTrak\StageImplementations

If there’s already a file with the same name in the “StageImplementations” folder, go ahead and overwrite it.

…And that’s it! You’re ready to try out this example protocol.

**<span style="text-decoration:underline;">General Guidelines:</span>**

**Session Length:**

30 minutes, twice daily, with a 2+ hour intersession interval.

**Feeding:**

Make sure each rat’s home cage food has been removed and that their cage has a completed food restriction card.  Prior to starting training, put half a scoop of Bio-Serv pellets into the rat’s home cage to acclimate them to the food, otherwise they won’t trust the unfamiliar food during their first training session (neophobia). If the rat didn’t receive at least 150 pellets combined across the morning and afternoon sessions, feed the rat two full size home cage food pellets or half a scoop of Bio-Serv/Purina pellets. If you notice rats dropping weight quickly, let your study leader know! At the end of the week (after last session on Friday) all rats should have full feed in their home cages.

**Habituation/Hand Training:**

Naive rats should be handled for ~15 minutes each every day for a week after arrival. Handling and hand training can be done on the same days the rats start shaping on MotoTrak behavior.



**<span style="text-decoration:underline;">Shaping Step 1 (1-2 days):</span>**


<table>
  <tr>
   <td>PURPOSE:
   </td>
   <td>Train the rat to associate interaction with the pull handle with a food reward.
   </td>
  </tr>
  <tr>
   <td>STAGE:
   </td>
   <td>P1
   </td>
  </tr>
  <tr>
   <td>MODULE POSITION:
   </td>
   <td>-0.5 cm (the pull handle will be easily accessible, protruding 0.5 cm into the cage)
   </td>
  </tr>
  <tr>
   <td>HIT THRESHOLD:
   </td>
   <td>Static, 10 gm
   </td>
  </tr>
  <tr>
   <td>DESCRIPTION:
   </td>
   <td>For the first session, simply leave the rat to explore the cage. Try to avoid making loud distracting noises outside the cage. Often, the rat will spontaneously learn to interact with the pull handle. After 2 sessions, if the rat hasn’t spontaneously learned to interact with the pull handle, you can entice the rat by placing crushed pellet powder on or near the pull handle. The rat will then lick or bite the pull handle, and in the process will trigger feeding. This should lead to association.
   </td>
  </tr>
  <tr>
   <td>PROGRESSION:
   </td>
   <td>The rat is ready to progress to Step 2 as soon as it is clear an association has been made between feeding and the pull handle. A good rule of thumb is that 50 feedings in one session indicates successful association.
   </td>
  </tr>
</table>




**<span style="text-decoration:underline;">Training Step 2 (2-10 sessions):</span>**


<table>
  <tr>
   <td>PURPOSE:
   </td>
   <td>Train the rat to reach outside the cage to interact with the pull handle, and to pull with increasing force.
   </td>
  </tr>
  <tr>
   <td>STAGE:
   </td>
   <td>P2
   </td>
  </tr>
  <tr>
   <td>MODULE POSITION:
   </td>
   <td>0.0 cm (even with the inner cage wall surface), automatically advancing to 2.0 cm as the rat learns the task.
   </td>
  </tr>
  <tr>
   <td>HIT THRESHOLD:
   </td>
   <td>Adaptive, between 10 gm (minimum) to 50 gm (maximum)
   </td>
  </tr>
  <tr>
   <td>DESCRIPTION:
   </td>
   <td>In this step, we’ll start to train the rat to reach outside the cage, restricted to the left or right paw, to interact with the pull handle. For the first trials, similar to the shaping step, almost any light pull on the handle will trigger feeding. After the first 10 trials of each session the program will start adaptively setting the hit threshold for the next trial based on the median peak pull force from the previous 10 trials (50th percentile). As the rat begins to pull with more force, the hit thresholds will increase, up to a maximum of 50 gm. If the rat performs badly, the hit threshold will decrease to keep them motivated, such that they are rewarded on ~50% of trials, on average.
   </td>
  </tr>
  <tr>
   <td>PROGRESSION:
   </td>
   <td>The rat is ready to progress to Step 3 when they are consistently pulling with more than 50 grams of force for 50 trials in a row with the module at a distance of 2.0 cm.
   </td>
  </tr>
</table>


**<span style="text-decoration:underline;">Training Step 3 (2-10 sessions):</span>**


<table>
  <tr>
   <td>PURPOSE:
   </td>
   <td>Train the rat to reach to full extension outside the cage and to pull with at least 120 grams of force.
   </td>
  </tr>
  <tr>
   <td>STAGE:
   </td>
   <td>P3
   </td>
  </tr>
  <tr>
   <td>MODULE POSITION:
   </td>
   <td>2.0 cm (the pull handle will be 2.0 cm outside the cage, measured from the inner wall surface)
   </td>
  </tr>
  <tr>
   <td>HIT THRESHOLD:
   </td>
   <td>Adaptive, between 50 gm (minimum) to 120 gm (maximum)
   </td>
  </tr>
  <tr>
   <td>DESCRIPTION:
   </td>
   <td>In this step, we’ll start to train the rat to reach outside the cage, restricted to the left or right paw, to interact with the pull handle in its final position. The hit threshold will start at 50 gm for the first 10 trials of each session, and the program will then start adaptively setting the hit threshold for the next trial based on the median peak pull force from the previous 10 trials. As in the previous training step, when the rat pulls with more force, the hit thresholds will increase, and if the rat performs badly, the hit threshold will decrease to keep them motivated.
   </td>
  </tr>
  <tr>
   <td>PROGRESSION:
   </td>
   <td>The rat is ready to progress to the Step 4, testing, when they are consistently pulling with more than 120 grams of force on 75% of trials.
   </td>
  </tr>
</table>


**<span style="text-decoration:underline;">Training/Testing Step 4 (10+ sessions):</span>**


<table>
  <tr>
   <td>PURPOSE:
   </td>
   <td>Test the rat’s isometric pull performance with full reach extension and a static 120 gram hit threshold.
   </td>
  </tr>
  <tr>
   <td>STAGE:
   </td>
   <td>P4
   </td>
  </tr>
  <tr>
   <td>MODULE POSITION:
   </td>
   <td>2.0 cm (the pull handle will be 2.0 cm outside the cage, measured from the inner wall surface)
   </td>
  </tr>
  <tr>
   <td>HIT THRESHOLD:
   </td>
   <td>Static, 120 gm
   </td>
  </tr>
  <tr>
   <td>DESCRIPTION:
   </td>
   <td>The final step is to capture a stable dataset to serve as your pre-injury/pre-intervention baseline. In each session, the hit threshold will be 120 grams for every trial, and the rat will have to reach with a full extension to the pull handle. Overall session hit rate, i.e. the percent of trials in which the animal exceeds the 120 gm hit threshold, is the primary datapoint to watch. Rats may be continuing to learn the task in Step 4 and hit rates may take several sessions to stabilize.
   </td>
  </tr>
  <tr>
   <td>PROGRESSION:
   </td>
   <td>The rat is considered fully trained and ready for injury/intervention when their hit rate is 75% or greater, on average, for 5 consecutive days (~10 sessions).
   </td>
  </tr>
</table>


**<span style="text-decoration:underline;">Daily Checklist:</span>**



* Did you weigh the rat prior to training/testing?
* Are any feeder LEDs blinking red to indicate a feeding error/no pellets?
* Are the feeder tubes properly connected to the feeder and cage?
* Did you spell the rat’s name correctly in the program?
* Is the signal shown on the MotoTrak program showing zero force when none is applied?

**<span style="text-decoration:underline;">Tips & Tricks:</span>**



* Create duplicate training stages with identical parameters, but different descriptions, to organize rats’ sessions according to their progression in the study. For example, you could create a copy of training/testing stage “P4: Pull Criterion Testing” and name it “P5: Post-Lesion Testing” to indicate sessions that occur after an injury model.
