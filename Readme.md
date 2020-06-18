# Book recommendations with Kubeflow Pipelines on Scaleway Kapsule

This repository contain the jupyter notebook example used for our Scaleway talk with Kevin Messy (in French) "Intégrer de l’IA dans votre SaaS : Nos conseils pour optimiser votre productivité et vos coûts"

## Goals of this demo

- Simple example suitable for a first overview of Kubeflow Pipelines 
- Simple demo to fit with the timing of the presentation
- Ditactic example to show how to use Kubeflow Pipelines with NFS storage and GPU
- This code is an example and not intended for production usage (Especially, no Serving modules has been implemented here)
- One of the goal of this demo was to demonstrate the possible gain of using GPU node pools with Autoscaling on Scaleway Kapsule (Managed Kubernetes)


## Book recommendation

This demo is reusing the code from Olga Petrova's blog post "[CPU or GPU for your recommendation engine?](https://blog.scaleway.com/2020/cpu-or-gpu-for-your-recommendation-engine/). (based on « NearestNeighbors » algorithm). 

This source code has been reused in a Jupyter Notebook in order to build and execute a simple Kubeflow Pipeline to illustrate the goals from this talk.


## How to use

In order to execute this notebook, you will need a Kubernetes cluster with Kubeflow 1.0 deployed on it. 

A Scaleway tutorial will be available shortly to describe the installation process on Scaleway Kapsule. By the time, a preliminary document is included in this repository in order to describe the installation procedure (See "Setup-Kubeflow-on-Kapsule-(draft).pdf" document). 

Once you have a Kubeflow cluster available, upload the Jupyter notebook in the Jupyter Hub, and execute it. Results are displayed in the pipeline task (K8S pod) logs, that you can access from the Kubeflow Pipeline GUI.


