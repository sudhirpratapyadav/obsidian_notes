
## Data collection
- Data should be even
- Some noise - cover state space around the optimal trajectories
	- keep increasing noise until success rate doesn't go below 90
- well distributed
- normalised
- Success rate should be high (90)
- Visualise dataset 
	- stats - distribution of states, actions, rewards etc
	- trajectories

## Training Procedure - Once data is fixed
- Important Params
	- Learning Rate
	- Batch Size
- Start with low batch size and low learning rate
	- This will require to train for more number of steps
	- keep on training until you get stable success rate or training become unstable (things going to inf)
- Then once you get success
	- increase batch size and learning rate -> this will make training faster
	- keep increasing until performance doesn't degrade
