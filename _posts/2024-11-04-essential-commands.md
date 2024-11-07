---
layout: post
title: Essential Commands for Docker, Hugging Face CLI, Git, and Vim
date: 2024-11-04 10:00:00
description: A practical guide with frequently used commands across Docker, Hugging Face CLI, Git, and Vim.
tags: 
categories: code
featured: false
---

This post provides a collection of essential commands for Docker, Hugging Face CLI, Git, and Vim, along with brief descriptions of their purpose and usage. These commands are organized for easy reference and formatted to suit common use cases.

---

## Docker Commands

Docker commands are essential for building, managing, and deploying containerized applications. Below are frequently used commands and their purposes.

#### 1. Build Docker Image

Build a Docker image from a specified `Dockerfile` with a custom tag.

```shell
docker build -t your-username/image-name:tag -f /path/to/Dockerfile .
```

- `-t` assigns a tag to the image.
- `-f` specifies the path to the `Dockerfile`.

#### 2. Run Docker Container

Runs a Docker container interactively with GPU support and mounts a local directory into the container.

```shell
docker run --rm -it --gpus all \
    -v /path/to/local/dir:/app \
    your-username/image-name:tag
```

- `--gpus all` allocates all available GPUs.
- `-v` mounts `/path/to/local/dir` to `/app` in the container.
  
#### 3. List Docker Images and Containers

List all Docker images and running containers.

```shell
docker images   # Lists all Docker images
docker ps       # Lists running containers
docker ps -a    # Lists all containers, including stopped ones
```

#### 4. Delete Docker Image and Clean Up

Delete a specific image and remove unused Docker resources.

```shell
docker rmi your-username/image-name:tag  # Deletes specified image
docker system prune                      # Cleans up unused resources
```

---

## Hugging Face CLI Commands

The Hugging Face CLI is useful for managing models and datasets. Below are commands for uploading, downloading, and managing files.

#### 1. Set Hugging Face Authentication Token

Set the Hugging Face token for authentication.

```shell
export HF_TOKEN="your_hf_token_here"
```

#### 2. Upload Files to Hugging Face Repository

Upload local files to a Hugging Face model or dataset repository.

```shell
huggingface-cli upload your-repo-name path/to/local/file1 path/to/repository/file1
```

#### 3. Download Files from Hugging Face Repository

Download files from a Hugging Face repository to a specified local directory.

```shell
huggingface-cli download your-repo-name path/to/repository/file1 --local-dir /path/to/local/dir
```

#### 4. Delete Files from Hugging Face Repository

Delete files from a Hugging Face repository.

```shell
huggingface-cli repo-files your-repo-name delete path/to/repository/file1
```

---

## TensorBoard to WANDB

The following commands allow you to sync TensorBoard logs to Weights and Biases (WANDB) for easy experiment tracking.

#### 1. Set WANDB API Key

Set your WANDB API key to authenticate with the service.

```shell
export WANDB_API_KEY="your_wandb_api_key_here"
```

#### 2. Sync TensorBoard Logs with WANDB

Sync your TensorBoard logs with a specified WANDB project.

```shell
python -c "import wandb; wandb.init(project='project-name')"
wandb sync /path/to/tensorboard/logs -p project-name
```

---

## Git Commands

Git commands are essential for version control. Below are some useful Git commands for managing changes, commits, and branches.

#### 1. Pull with Local Changes

Allows pulling changes while keeping specific files unchanged. Useful when you want to avoid overwriting local modifications.

```shell
git update-index --skip-worktree path/to/file1 path/to/file2
git pull
git update-index --no-skip-worktree path/to/file1 path/to/file2
```

#### 2. Revert Last Commit

Undo the last commit, with options to either keep or discard the changes made in that commit.

```shell
git reset --hard HEAD~1  # Remove commit and changes
git reset --soft HEAD~1  # Remove commit but keep changes staged
git commit -m "New commit message"
git push origin <branch_name> --force
```

#### 3. List All Branches

View all branches in the repository.

```shell
git branch           # List local branches
git branch -r        # List remote branches
git branch -a        # List all branches, local and remote
```

---

## Vim Commands

Vim is a powerful text editor with efficient shortcuts for navigating and editing files. Below are some commonly used Vim commands.

#### 1. Enter Visual Mode and Copy Text

Use visual mode to select and copy (yank) text.

```vim
v         # Enter visual mode
y         # Yank (copy) selected text
```

#### 2. Search and Navigate in File

Use search to locate text in a file.

```vim
/word     # Search for "word"
n         # Jump to the next occurrence
N         # Jump to the previous occurrence
esc       # Exit search mode
```

#### 3. Save and Exit

Common commands for saving and exiting Vim.

```vim
:w         # Save changes
:q         # Quit
:wq        # Save and quit
:q!        # Quit without saving
```

---
