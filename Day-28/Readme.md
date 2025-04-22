Day 28 Task: Jenkins Agents

Jenkins Master (Server)

Jenkins’s server or master node holds all key configurations. Jenkins master server is like a control server that orchestrates all the workflow defined in the pipelines. For example, scheduling a job, monitoring the jobs, etc.

Jenkins Agent

An agent is typically a machine or container that connects to a Jenkins master and this agent that actually execute all the steps mentioned in a Job. When you create a Jenkins job, you have to assign an agent to it. Every agent has a label as a unique identifier.

When you trigger a Jenkins job from the master, the actual execution happens on the agent node that is configured in the job.

A single, monolithic Jenkins installation can work great for a small team with a relatively small number of projects. As your needs grow, however, it often becomes necessary to scale up. Jenkins provides a way to do this called “master to agent connection.” Instead of serving the Jenkins UI and running build jobs all on a single system, you can provide Jenkins with agents to handle the execution of jobs while the master serves the Jenkins UI and acts as a control node.



Pre-requisites

Let’s say we’re starting with a fresh Ubuntu 22.04 Linux installation. To get an agent working make sure you install Java ( same version as jenkins master server ) and Docker on it.

Note:- While creating an agent, be sure to separate rights, permissions, and ownership for jenkins users. 

Task-01
- Create an agent by setting up a node on Jenkins

- Create a new AWS EC2 Instance and connect it to master(Where Jenkins is installed)

- The connection of master and agent requires SSH and the public-private key pair exchange.

- Verify its status under "Nodes" section.

- You can follow this article for the same

Task-02
- Run your previous Jobs (which you built on Day 26, and Day 27) on the new agent

- Use labels for the agent, your master server should trigger builds for the agent server.

