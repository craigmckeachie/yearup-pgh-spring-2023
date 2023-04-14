# Git Workflow using Visual Studio Code (GUI) and starting with Code on your Computer

# Local Repository

## Objectives

- Start your project and write some code
- Save a snapshot (commit) of your initial code
- Write more code and save additional snapshots (commits) of the code frequently

## Steps

### Start your project and write some code

1. Create a directory on your machine to store your code for a project. We will call this the `project directory`.

   ![1a](https://user-images.githubusercontent.com/1474579/231314469-1fabb5d7-188b-4988-888c-51fa523954f0.png)

   ![1b](https://user-images.githubusercontent.com/1474579/231314715-87bd3bdd-0596-4fcf-96ba-632837efe4a1.png)

1. Open the project directory in VS Code.

   > Note: Be sure to use `File > Close Folder` to close any other directories you have open before opening a new directory.

   ![image](https://user-images.githubusercontent.com/1474579/231316290-b769ab7d-585d-49ed-a8a3-d4e851a2c62c.png)

   ![image](https://user-images.githubusercontent.com/1474579/231316655-cfa7bd9d-c758-470c-8b51-8262d96fe393.png)

1. Add some intial files to your project directory.

   ![image](https://user-images.githubusercontent.com/1474579/231316741-a27b8149-a7bb-4405-b446-35cf00d032b6.png)

### Save a snapshot of your initial code

1. Initialize a local git repository (database).

   ![image](https://user-images.githubusercontent.com/1474579/231316878-a4a4a5e6-6517-4c4b-a355-4ca3824d50ff.png)

1. Stage your changes to the local git repository.

   ![image](https://user-images.githubusercontent.com/1474579/231317934-bafc2bc1-cfb5-4564-9e5a-d9b2df80ec8d.png)

1. Add a message and commit your staged changes to the local git repository.

   ![image](https://user-images.githubusercontent.com/1474579/231318265-890c8710-1927-4c0b-8a7c-185756151913.png)

1. View your commit.

   ![image](https://user-images.githubusercontent.com/1474579/231318955-83cfe60c-ad17-42b5-a0f6-ec229a97f79b.png)

### Write more code and save additional snapshots of the code frequently

1. Continue to develop and change files, delete files or add files.
1. Stage your change to the local git repository.

   ![image](https://user-images.githubusercontent.com/1474579/231317934-bafc2bc1-cfb5-4564-9e5a-d9b2df80ec8d.png)

1. Add another message and commit your changes to the local git repository.

   ![image](https://user-images.githubusercontent.com/1474579/231319252-d36d9c54-35e5-45e5-a7aa-effaae4fa907.png)

> Note: these last 3 steps can be repeated over and over after the project is setup to take additional snapshots (commits)

### &#10004; You have committed changes to a local Git repository

<br>

---

# Remote Repository

## Objectives

- Push/Publish code to a remote repository

## Steps

### Push/Publish Code to a remote repository

1. **Click** the **"Publish Branch"** button
   <img width="453" alt="image" src="https://user-images.githubusercontent.com/1474579/231914157-4d8f0149-121b-4669-ac02-197ca2add8ed.png">

2. **Choose** to create a **"Public Repository"**
   <img width="1258" alt="image" src="https://user-images.githubusercontent.com/1474579/231914647-0fd26735-aeff-4083-9d4e-47843ae35f9b.png">

   > Note: the publish button will only be shown if you have no working and/or staging files

   > Tip: You can choose the three dots in the menu and choose the **Push** action to publish when you have files that are in working or staging

   <img width="767" alt="image" src="https://user-images.githubusercontent.com/1474579/231915251-168e4622-594d-475a-ae36-bc838b28e605.png">
