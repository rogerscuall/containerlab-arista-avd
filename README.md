# Containerlab and Arista AVD

This repo has a setup to use [Containerlab](https://containerlab.dev/) and Arista [AVD](https://avd.sh/).

[AVD](https://github.com/aristanetworks/ansible-avd) has a few examples under `ansible_collections/arista/avd/examples/`, the following repo has updated this example to be used with Containerlab.

## Requirements

* Containerlab [Containerlab Installation](https://containerlab.dev/install/)

## How to use

The following steps are very similar to all the labs, we will use **single-dc-l3ls** int this case:
1. Move to the folder for the example: `cd single-dc-l3ls`.
1. Create a virtual environment and activate it.
1. Install the requirements: `pip install -r requirements.txt`
1. Install the galaxy dependencies: `ansible-galaxy collection install arista.avd`
1. Deploy containerlab: `sudo containerlab deploy`
1. Run the build `ansible-playbook build.yml`
1. Run the deploy `ansible-playbook deploy.yml`