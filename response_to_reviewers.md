First, I want to thank the reviewers for their thorough reviews. It was nice to hear that the project seems to be a good showcase for julia.

I changed the following things according to comments:

* General: typos in various places
* fbs.ipynb:
  * added a non-interactive version of the plot where the user can still try out different parameters by changing the code cell in case WebIO doesn't work
  * added a note that there is no problem if the interactive plot doesn't work
* I included a sentence on running the notebook either sequentially or via 'Run->Run all cells' in the readme
* I added a few words in evaluation.ipynb where the contents of the csv files are explained to clear up what T_RL and E are.

I chose not to change a few things commented on for the following reasons:

* Title, Abstract, relation of the notebooks: the introduction in the readme already states that fbs.ipynb is used to find a parameter for a more advanced simulation and evaluation.ipynb is used to evaluate output from that advanced simulation.
* dimension of the plots: since there is always the option to save the plots as pdf i.e. in a vector format the resolution will not be a problem (the heatmaps will be embedded with the "resolution" of the data array)
* The energy scales here are very small and as a matter of fact they are here usually scaled in terms of other quantities
* I couldn't identify what part of the abstract is unclear. This is meant as supplement to a (not yet published) bigger work, that would put things into context. I think there is not really a way to solve this without an unreasonable amount of additional/double effort.
* The size of the saved plots doesn't play a big role since they can be saved as pdf where the line plots are saved as vectors, so they scale loss free. The heatmaps are saved with "native resolution" i.e. all the pixels the array provides. (the 'size=...' argument in the plot command in julia does afaik only influence the proportion of the figure that is saved, so it's kind of irrelevant)

Again thanks for the constructive feedback!
