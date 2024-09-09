# Policy Diversity by Neuroevolution

The following agents either move in ways that humans would expect or in ways that humans would not expect. 
Some agents are very aggressive, while others are lazy. Some agents have one or more joints that remain stationary. 
Even when these joints fail, the agents can still move normally, 
which allows them to better cope with dynamically changing environments and increase robustness.

## Three diverse agents of Walker2D


<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/walker1_cso.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CSO, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 4460.

Only the agent's left leg and right foot are moving significantly, but the right knee joint is not moving.</p>
    </div>
</div>


<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/walker2_cso.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CSO, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 3124.

Only the left knee joint and right ankle joint of the agent are shaking slightly, and the left foot and right leg are not moving. 
And the right foot maintains the minimum contact area with the ground to reduce friction, making this movement possible.</p>
    </div>
</div>


<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/walker3_cso.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CSO, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 2648.

This agent moves in the same way as the previous agent, but the distance between its two legs is greater.
</p>
    </div>
</div>


## Four diverse agents of Hopper

<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/hopper1_cso.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CSO, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 3344.

The first joint and ankle joint of the agent's leg move, while the second joint remains stationary. 
When jumping forward, the first and second joints may remain perpendicular to the ground.</p>
    </div>
</div>


<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/hopper2_cmaes.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CMAES, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 3529.

The first joint and ankle joint of the agent's leg move, while the second joint remains stationary. 
The first joint and ankle joint of the agent's leg are moving, while the second joint remains stationary. 
This movement is the same as the previous agent, but because the first and second joints maintain a certain angle 
between them and are tilted forward relative to the ankle joint, the jumping distance is greater, 
which is the same as the way humans jump.</p>
    </div>
</div>


<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/hopper3_cmaes.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CMAES, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 3492.

The second joint and ankle joint of the agent's leg are moving, while the first joint remains stationary. 
The part above the second joint has a slight tendency to lean forward and backward.</p>
    </div>
</div>

<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/hopper4_cmaes.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CMAES, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 3614.

The second joint and ankle joint of the agent's leg are moving, while the first joint remains stationary. 
This movement is the same as the previous agent, but the upper part of the second joint remains perpendicular to the ground, 
which reduces swing and allows for faster jumps.</p>
    </div>
</div>

## Four diverse agents of HalfCheetah

<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/halfcheetah1_cso.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CSO, where popsize=1000, iterations=1000, hidden={16, 16}. The reward is 9540.

Although the running posture of this agent looks normal, the coordination between 
its front and rear legs is not very coordinated, and the swing range of the front leg knee joint is very small.
</p>
    </div>
</div>

<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/halfcheetah5_cmaes.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for CMAES, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 16674.

The front and rear legs of the agent work very well together, so it runs faster than the agent in front.</p>
    </div>
</div>

<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/halfcheetah2_cso.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for NCG-CSO, where popsize=1000, iterations=1000, hidden={16, 16}. The reward is 6412.

The agent's backward movement is in an unexpected way.
</p>
    </div>
</div>

<div style="display: flex; align-items: center; margin-bottom: 40px;">
    <img src="./figures/halfcheetah3_cso_.gif" alt="Visualization of the policy" width="300" height="300" style="margin-right: 20px;">
    <div>
        <p>This is the result for CSO, where popsize=100, iterations=10000, hidden={16, 16}. The reward is 6891.

After falling down with a somersault, 
the agent moved forward by lying down with the help of the coordination of its head and legs.
</p>
    </div>
</div>

