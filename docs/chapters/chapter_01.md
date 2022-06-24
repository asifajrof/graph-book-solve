# Graphs and Their Applications

## Exercises

### 1.
Study your campus map and model the road network inside your campus by a graph.

**Answer:** \[Do it yourself\]

### 2.
Construct a graph to represent the adjacency relationship of rooms in a floor of your university building.

**Answer:** \[Do it yourself\]  
Some examples taken from a floor plan paper \[[2]\] in Figure [1.2.1]

<figure>
<embed src="../../figures/1_2_floorplan_to_graph.svg" id="fig:1_2_floorplan_to_graph"
style="width:100.0%" />
<figcaption aria-hidden="true">Floor plan</figcaption>
</figure>

### 3.
Consider a party where there are exactly two alternate options of foods for each category of foods as follows. Rice: plane/yellow, Curry: fish/chicken, Naan: plain/butter, Kebab: chicken/mutton, Fruit: banana/mango, Drink: tea/coffee. Registered participants of the party gave their options as in Figure [1.3.1]. Two participants conflict in their options if they give different options in the same category. Represent the conflicts of the participants using a conflict graph where each participant is represented by a vertex and there is an edge between two vertices if the corresponding participants conflict. By observing the conflict graph, find out the minimum number of persons whose absence divides the participants into two conflict free groups.

<figure>
<embed src="../../figures/1_3_table_food_opt.svg" id="fig:1_3_table_food_opt"
style="width:100.0%" />
<figcaption aria-hidden="true">Food option</figcaption>
</figure>

**Answer:** Conflict graph Figure [1.3.2]
<figure>
<embed src="../../figures/1_3_conflict_graph.svg" id="fig:1_3_conflict_graph"
style="width:100.0%" />
<figcaption aria-hidden="true">Conflict graph</figcaption>
</figure>

Conflict free groups: {Abir, Dristy, Faria, Jony}, {Bony, Elis},
{Subir}, {Snigdha}.  
Exclude 2 persons namely Subir and Snigdha to get two conflict free
groups {Abir, Dristy, Faria, Jony} and {Bony, Elis}

### 4.
There are five jobs $\{J_1, J_2, J_3, J_4, J_5\}$ in a company for which there are five workers $A, B, C, D$ and $E$ to do those jobs. However, everybody does not have expertise to do every job. Their expertise is as follows: $A = \{J_1, J_2, J_3\}$, $B = \{J_2, J_4\}$, $C = \{J_1, J_3, J_5\}$, $D = \{J_3, J_5\}$, $E = \{J_1, J_5\}$. Develop a graph model to represent the job expertise of the persons and find an assignment of jobs to the workers such that every worker can do a job.

**Answer:** Job assignment graph Figure [1.4.1]

<figure>
<embed src="../../figures/1_4_job_assg.svg" id="fig:1_4_job_assg"
style="width:100.0%" />
<figcaption aria-hidden="true">Job assignment graph</figcaption>
</figure>

### 5.
An industry has 600 square meter rectangular area on a floor of a building where it needs to establish four processing units $A, B, C$, and $D$. Processing units $A$ and $D$ require 100 square meter area each whereas $B$ and $C$ require 200 square meter each. Furthermore, the following adjacency requirements must be satisfied: $B, C$, and $D$ should be adjacent to $A; A$ and $D$ should be adjacent to $B; A$ and $D$ should be adjacent to $C;$ and $A, B$, and $C$ should be adjacent to $D$. Can you construct a floor layout where the space for each processing unit will be a rectangle? Propose a suitable layout in your justification.

**Answer:** Industry unit layout Figure [1.5.1]

<figure>
<embed src="../../figures/1_5_floor_plan.svg" id="fig:1_5_floor_plan"
style="width:80.0%" />
<figcaption aria-hidden="true">Industry unit layout</figcaption>
</figure>

[2]: ../../references/#ref2
[1.2.1]: #fig:1_2_floorplan_to_graph
[1.3.1]: #fig:1_3_table_food_opt
[1.3.2]: #fig:1_3_conflict_graph
[1.4.1]: #fig:1_4_job_assg
[1.5.1]: #fig:1_5_floor_plan