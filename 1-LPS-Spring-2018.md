# 1 L/s Plant Testing
#### Sung Min Kim, Sidney Lok, Erica Marroquin
#### March 9, 2018

# Manual
The goal of this section is to provide all of the guidance that would be necessary for a future team to pick up your work where you left off. Please try to be thorough and put yourselves in the shoes of a newcomer to the project. Below are some recommended sections, but the manual will likely take a slightly different form for each team.

## Fabrication Details
Include any information related to the fabrication of equipment, experimental apparatuses, or technologies. Include the purpose of each step and the fabrication methods used. Reference appropriate safety precautions.

### Lever Arm Perforation
One of the first tasks the team had to complete was securing the lever arm onto the side of the entrance tank. At the beginning of the semester, the lever arm and entrance tank were still separate pieces as shown in Figures 1 and 2. At this point, the lever arm could slide into the hole in Figure 1 made on the attachment at the side of the entrance tank, but there was no way to ensure that the lever arm would not slide out of the hole.

![Hole at side of entrance tank](https://photos.app.goo.gl/QzVMZvVbbzi6H7s33)
Figure 1: There is a hole in the PVC bar attachment at the side of the entrance tank. This is where the lever arm slides in.

![Lever Arm before](https://photos.app.goo.gl/vwRi7EAqTxyBxAW82)
Figure 2: Pictured is the lever arm before modification. Note that there is no visible way of securing the lever arm in place after sliding the metal bar into the hole at the side of the entrance tank shown in Figure 1.

The team consulted AguaClara Engineer Juan Guzman and determined that a perforation should be made in the metal bar of the lever arm so that a pin could be placed inside of it and act as a stopper as illustrated in Figure 3.

![Lever Arm Schematic](https://photos.app.goo.gl/gcuF4lbcbVELAUw72)
Figure 3: Shown is a schematic of how the lever arm should fit onto the entrance tank. There should be a perforation in the metal bar of the lever arm in order for a pin to fit inside and act as a stopper. After being slid into the hole shown in Figure 1, a pin should be inserted into the perforation to secure the lever arm onto the entrance tank.

The team first found a piece to act as a pin and determined the size of it. The lever arm was brought to Timothy Brock in the Hollister Hall Machine Shop and perforated according to the size of the pin using a mill as shown in Figure 4. The pin fit snugly into the perforation as shown in Figure 5.

![Lever Arm being perforated](https://photos.app.goo.gl/0Svr6cGOvz6PyiPJ3)
Figure 4: Timothy Brock used a mill machine in the Machine Shop to perforate the metal bar.

![Metal bar after perforation](https://photos.app.goo.gl/UaMVMCm7cPt1brKq2)
Figure 5: The pin fit snugly into the perforation because the team had measured the pin beforehand and determined the size of it.

##CDC Apparatus
During summer 2017, AguaClara fabricated a new design of the chemical dose controller (CDC). The original design can be found [here](https://www.overleaf.com/read/zfcbvtrykhwc#/28982452/) and the summer report [here](URL). The CDC system was designed to maintain a constant chemical dose to the treatment process as the plant flow rate and influent turbidity change. The main difference from the two designs is that slimmer PVC pipes were used. The current CDC system is incomplete for chlorination as shown in Figure x but is complete for the team's testing this semester.

The CDC works in conjunction with the lever arm on the side of the entrance tank. The team has to ensure that the height of the lever arm when horizontal is the same as the coagulant level of the CDC when the float values are submerged. Because running the 1 L/s plant first with water was the priority, the team has not properly made sure that the heights were equal on the pole. The team plans to match the heights as shown in Figure x after assembling all the materials needed for the coagulant run.

##1 L/s Plant Water Run
The team's main focus was to run water through the 1 L/s plant, from the entrance tank to the flocculators. Ideally the team would run the plant with the EStaRs but because it had not been tested, the team is separately troubleshooting and water testing the EStaRs.

##EStaRs Testing
According to the team that worked on the EStaRs filter during summer 2017, the filter had been water tested. The team added sand to the filter and checked the top and bottom filter seals. However, there are a few leaks in the welds under the exit tank and the team took apart the piping to check the inside welds as shown in Figure x.


## Special Components
If your subteam uses a particular part that is unique and you could foresee a future subteam needing to order it or learn more about it, please include basic information like the vendor where it was purchased, catalog/item number, and a link to any documentation.

## Experimental Methods
### Set-up
Step 1.
* Put tasks in a sequential order.
* It is okay to have sub-lists.
  - Like this.

### Experiment
Step 1.

### Cleaning Procedure
Step 1.

## Experimental Checklist
Another potential section could include a list of things that you need to check before running an experiment.

## ProCoDA Method File
Use this section to explain your method file. This could be broken up into several components as shown below:

### States
Here, you should describe the function of each state in your method file, both in terms of its overall purpose and also in terms of the details that make it distinct from other states. For example:
\begin{itemize}
\item \underline{OFF} - Resting state of ProCoDA. All sensors, relays, and pumps are turned off.
\end{itemize}

### Set Points
Here, you should list the set points used in your method file and explain their use as well as how each was calculated.

## Python Code

### Variables
$g$: gravity
$\sigma$: dispersion
$a$: amplitude
$h$: water depth
$H$: distance from wave crest to trough (2$a$)
$T$: wave period
$\lambda$: wavelength
$k$: wavenumber
$c_p$: celerity (wave phase speed)
$P$: pressure
$F$: force
$u$, $w$: x-velocity, z-velocity components

```python
# Comment
```

# Add/Delete/Change this Template as you see Fit
When using this template keep in mind that this serves three purposes. The first is to provide your team feedback on your progress, assumptions, and conclusions. The second is to keep your team focused on what you are learning and doing for AguaClara. Another is to educate future teams on what you've learned and done. This document should be comprehensive, consistent, and well-written. With that in mind, add, subtract, or move sections. Reach out to the RAs and graders for help with figuring out what should or shouldn't include. Focus on how wonderful a reference you are making through this and work hard on communicating amongst yourselves and with future teammates. (Delete this section before submitting)

```python
# To convert the document from markdown to pdf
pandoc Name_of_this_file.md -o TeamName_Research_Report.pdf
```
